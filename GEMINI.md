# GEMINI.md

## Project Overview

This is a Vue.js project bootstrapped with Vite. It appears to be a learning and demonstration repository containing a large number of Vue components that showcase various features of the Vue 3 framework.

The project is structured with a clear separation of concerns, containing directories for components, new components, pages, router, stores, utils, and views.

**Key Technologies:**

*   **Framework:** Vue 3
*   **Build Tool:** Vite
*   **Routing:** Vue Router
*   **State Management:** Pinia
*   **UI Library:** Element Plus
*   **Other Libraries:** Swiper.js for carousels, Axios for HTTP requests.

The application's entry point is `src/main.js`, where Vue, Vue Router, Pinia, and Element Plus are initialized. The root component is `src/App.vue`, which sets up the main layout and a router view. The project contains a wide variety of components demonstrating everything from basic template syntax and event handling to more advanced concepts like dynamic components, slots, and integration with Pinia.

## Building and Running

You can manage the project using the scripts defined in `package.json`.

*   **To run the development server:**
    ```bash
    npm run dev
    ```

*   **To build the project for production:**
    ```bash
    npm run build
    ```

*   **To preview the production build:**
    ```bash
    npm run preview
    ```

## Development Conventions

*   **Component Structure:** The project contains a large number of Single File Components (`.vue` files).
*   **API Style:** There is a mix of both the Options API and the Composition API (`<script setup>`) used across different components. `App.vue` uses the Options API, while newer components might be using the Composition API.
*   **Styling:** Global styles are present in `src/App.vue`, and component-specific styles are likely co-located within the `.vue` files.
*   **Routing:** Routes are centrally managed in `src/router/index.js`.
*   **State Management:** Global state is handled by Pinia, with stores defined in the `src/stores` directory.
