

# Install vue-cli: 

* Run `npm install --global vue-cli`


# Create a new project using the "webpack" template

* Run `vue init webpack todo-app`

* Select which options you desire


# Install dependencies and go!

* Run `cd todo-app` and then `npm install`


# Serve the app

* Run `npm start`


# Installed Vetur extension in VSC

* Vetur

# Adding a component

* Create a new file within the components folder. And give it the basic component setup

    ```
    <template>
    <div>
        <h1></h1>
    </div>
    </template>

    <script type = "text/javascript" >

    export default {
    };
    </script>
    <style>
    </style>
    ```

* Import it into your App.vue file at the top of/but still within the script tags. 

    ```
    import NewComponent from './components/NewComponent'  
    ```

* Add a reference to the component in the components property
    
    ```
    <script>
        import TodoList from './components/NewComponent';

        export default {
        components: {
            NewComponent,
        },
        };
    </script>

    ```

* Render the component 

    ```
    <template>
    <div>
        <NewComponent/>>
    </div>
    </template>
    ```