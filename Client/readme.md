# Vue.js
# Estructura
```
project-root/
|-- src/
|   |-- assets/
|       |-- styles/
|   |-- components/
|       |-- TaskList.vue
|       |-- NotificationList.vue
|       |-- Statistics.vue
|   |-- views/
|       |-- Dashboard.vue
|   |-- services/
|       |-- ApiService.js
|       |-- NotificationService.js
|   |-- App.vue
|   |-- main.js
|-- public/
|-- package.json
|-- vue.config.js
```
# Componentes
```vue
<!--TaskList.vue-->
<template>
  <div>
    <h2>Task List</h2>
    <ul>
      <li v-for="task in tasks" :key="task.id">
        {{ task.title }} - {{ task.dueDate }}
      </li>
    </ul>
  </div>
</template>

<script>
export default {
  data() {
    return {
      tasks: [], // You'll populate this with data from the API
    };
  },
  mounted() {
    // Fetch tasks from the API using ApiService
    // Example: ApiService.getTasks().then(response => this.tasks = response.data);
  },
};
</script>

<style scoped>
/* Add your component-specific styles here */
</style>
```
```vue
<!--NotificationList.vue-->
<template>
  <div>
    <h2>Notification List</h2>
    <ul>
      <li v-for="notification in notifications" :key="notification.id">
        {{ notification.message }} - {{ notification.timestamp }}
      </li>
    </ul>
  </div>
</template>

<script>
export default {
  data() {
    return {
      notifications: [], // You'll populate this with data from the API
    };
  },
  mounted() {
    // Fetch notifications from the API using NotificationService
    // Example: NotificationService.getNotifications().then(response => this.notifications = response.data);
  },
};
</script>

<style scoped>
/* Add your component-specific styles here */
</style>
```
```vue
<!--Statistics.vue-->
<template>
  <div>
    <h2>Statistics</h2>
    <!-- Display various statistics here -->
  </div>
</template>

<script>
export default {
  // You can add data, methods, and lifecycle hooks as needed
};
</script>

<style scoped>
/* Add your component-specific styles here */
</style>
```
```vue
<!--Dashboard.vue-->
<template>
  <div>
    <task-list></task-list>
    <notification-list></notification-list>
    <statistics></statistics>
  </div>
</template>

<script>
import TaskList from '@/components/TaskList.vue';
import NotificationList from '@/components/NotificationList.vue';
import Statistics from '@/components/Statistics.vue';

export default {
  components: {
    TaskList,
    NotificationList,
    Statistics,
  },
};
</script>

<style scoped>
/* Add your view-specific styles here */
</style>
```
# To learn
- Vue Components
- Vue Router
- Vue Templates y Directivas
- Vue Services y Axios
- OPCIONAL Gestion de Estado con Vuex
- Manejo de Eventos y Emisores de Eventos
- Tailwind
- Responsive Design
- Conceptos Basicos de Seguridad en Frontend
- Build y Despliegue
