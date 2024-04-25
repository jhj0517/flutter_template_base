# Flutter Template Starter
This is the Flutter template starter with [mason](https://github.com/felangel/mason). 

# Platforms
The mustache syntax `{{application_id}}` is implemented across 6 platforms. Only Android has been tested. If any errors occur or if it works fine on other platforms, please raise an issue and let me know.
1. Android ✅ - 24.04.26
2. IOS ❓ - Not tested yet
3. Web ❓ - Not tested yet
4. Linux ❓ - Not tested yet
5. MacOS ❓ - Not tested yet
6. Windows ❓ - Not tested yet

# Prompts
There're 4 prompts for the brick.
1. `project_name` : Project name. Used for multiple platforms.
2. `org_name` : Organization name like `com.example`
3. `application_id` : App id after the organization name. Used on multiple platforms with `org_name`.
4. `description` : Project description.

# How to Make Template
1. Git clone this repository
   ```
   https://github.com/jhj0517/flutter_template_starter.git
   ```
2. Go to [project folder](https://github.com/jhj0517/flutter_template_starter/tree/master/flutter_template_starter/__brick__/%7B%7Bproject_name.snakeCase()%7D%7D) and make your own template.
3. Add the brick as the global (you can edit the brick name in `mason.yaml` as you want )
   ```
   mason add -g flutter_template_starter --path flutter_template_starter 
   ```
4. Check that the brick is added correctly.
    ```
    mason ls -g
    ├── flutter_template_starter 0.1.0  // it prints something like this
    ```
5. You can now start a new project with your own template
   ```
   mason make flutter_template_starter
   ```
