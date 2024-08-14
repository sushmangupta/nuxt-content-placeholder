# Project setup

Great! Now that you have Shopware instance ready, let's focus on setting up your local project with version control and an IDE (Integrated Development Environment). This setup will help you manage your code efficiently and streamline your development process.

## Organizing your Shopware project for version control

### IDE setup

Your IDE will be your primary tool for writing and debugging code, so it's essential to set it up correctly. For best use, its recommended to work on PHPStorm. However, you can also work on VS Code or any other similar IDE's.

#### PHPStorm Setup

PHPStorm is a popular IDE for PHP development, and it has excellent support for Shopware.

1. **Open Project**: Start by opening your Shopware project in PHPStorm.

2. **Configure PHP Interpreter**:

   - Go to `File > Settings > PHP` (or `PHPStorm > Preferences > PHP` on macOS).
   - Add a new local interpreter.
   - Point it to the location of your locally installed PHP executable (e.g., C:\xampp\php\php.exe on Windows or /usr/bin/php on Linux/Mac).

3. **Enable Xdebug** (Optional but recommended):

   - In the same PHP settings window, under "Debug," enable Xdebug.
   - Ensure your `docker-compose.yml` file has Xdebug configured.

   Xdebug is a PHP extension that provides powerful debugging, error handling and profiling capabilities.

4. **Configure Code Style**:

   - Shopware follows PSR-12 coding standards.
   - Go to `File > Settings > Editor > Code Style > PHP` and ensure the settings align with PSR-12.

5. **Set Up Shopware Plugin Development**:

   - Use the "Symfony" plugin in PHPStorm to recognize the Symfony framework components used by Shopware.
   - Configure the plugin path if you're developing custom plugins.

6. **Working with Git in PHPStorm**:

   - PHPStorm has built-in Git support. You can manage your version control directly from the IDE, including committing, branching, merging, and pushing changes.

#### VSCode Setup

VSCode is a lighter, free alternative to PHPStorm and also works well with Shopware.

1. **Open Project**: Open your Shopware project in VSCode.

2. **Install Extensions**:

   - **PHP Intelephense**: For PHP autocomplete and linting.
   - **PHP Debug**: For Xdebug integration.
   - **Symfony Support**: For recognizing Symfony components.
   - **EditorConfig**: Ensures consistent coding styles.
   - **ESLint**: For JavaScript/TypeScript linting (useful if you're working on frontend code).

3. **Configure PHP and Xdebug**:

   - Go to `File > Preferences > Settings` and search for `PHP`.
   - Point the PHP executable to the one inside your Docker container.
   - For Xdebug, configure a `launch.json` file for debugging:

   ```json
   {
       "version": "0.2.0",
       "configurations": [
           {
               "name": "Listen for Xdebug",
               "type": "php",
               "request": "launch",
               "port": 9003,
               "pathMappings": {
                   "/var/www/html": "${workspaceFolder}"
               }
           }
       ]
   }
   ```

4. **Git Integration**:

   - VSCode has built-in Git support, accessible from the Source Control tab. You can stage changes, commit, push, pull, and manage branches directly from within the editor.

### .gitignore Setup

When working with version control, it's essential to ensure that certain files and directories aren't included in your Git repository. These are typically files that are environment-specific or can be generated (like compiled code or vendor dependencies).

Shopware projects should have a `.gitignore` file that includes the following:

```plaintext
# Ignore Composer's vendor directory
/vendor/
/composer.lock

# Ignore Shopware's cache and logs
/var/cache/
/var/log/

# Ignore node_modules for frontend dependencies
/node_modules/

/public/bundles/
/public/media/
/public/thumbnail/
/public/theme/

/config/jwt/
/config/packages/local.yaml

# Ignore environment variables file
.env

# Ignore IDE configuration directories
.idea/
/.vscode/

# Ignore Docker and other development-related files
docker-compose.override.yml
```

## Setting Up the Repository

1. **Initialize Git**: If you haven't already done so, initialize your Git repository inside the Shopware project directory:

    ```bash
    git init
    ```

2. **Initial Commit**: Add all the necessary files to your repository and commit them:

    ```bash
    git add .
    git commit -m "Initial commit of Shopware project"
    ```

3. **Remote Repository**: If you’re using a remote repository service like GitHub, GitLab, or Bitbucket, create a new repository there and link it to your local repository:

    ```bash
    git remote add origin <your-repository-url>
    git push -u origin master
    ```

## Development Workflow

With version control and your IDE set up, here's a typical development workflow:

1. **Create a New Branch**: For any new feature or bug fix, create a new Git branch:

   ```bash
   git checkout -b feature/your-feature-name
   ```

2. **Develop Your Feature**:
   - Write code using your IDE. Use the integrated tools to check for coding standards, run tests, and debug.

3. **Commit Changes**: Regularly commit your changes with meaningful commit messages:

   ```bash
   git add .
   git commit -m "Implement feature X"
   ```

4. **Push Changes**: Push your branch to the remote repository:

   ```bash
   git push origin feature/your-feature-name
   ```

5. **Create a Pull Request**: On your Git hosting service (GitHub, GitLab, etc.), create a pull request to merge your changes into the main branch. Review and merge after approval.

6. **Deploy**: Depending on your deployment process, you can automate deployments through CI/CD pipelines or manually deploy by merging changes to a specific branch (e.g., `production` or `main`).

## Additional Tools

- **PHPUnit**: For unit testing your Shopware code, configure PHPUnit within your IDE for easy testing.
- **ESLint/Prettier**: For maintaining consistent code quality in JavaScript/TypeScript files.
- **Docker-compose.override.yml**: Use this file to customize your local Docker environment without affecting the main setup, especially useful for different environments (dev, staging, prod).

By following these guidelines, you will have a well-organized, efficient development environment that leverages the power of version control and modern IDE features. This setup not only improves productivity but also helps maintain code quality and consistency across the team.