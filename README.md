# Mini PHP Framework with MVC Architecture

## Description

This project is a mini PHP framework designed to follow the Model-View-Controller (MVC) architecture. It aims to provide a lightweight and easy-to-use structure for web application development, facilitating separation of business logic, user interface, and flow control, thereby enhancing code maintainability and scalability.

## Key Features

- **MVC Architecture**: Organizes the application into three main components: Model, View, and Controller.
- **Routing**: Simple routing system mapping URLs to specific controllers and methods.
- **Autoloading**: Automatic class loading using the PSR-4 standard to simplify dependency management.
- **Error Handling**: Centralized error handling for better exception management and debugging.
- **Template Support**: Integration with a template engine to separate presentation logic from PHP code.
- **Flexible Configuration**: Configuration file to define routes, database connectivity, and other key settings.

## Project Structure

- **Assets**: Contains all static assets.
  - **css**: Stylesheets (e.g., `style.css`).
  - **images**: Image files.
  - **js**: JavaScript files.
    - **plugins**: JavaScript plugins.

- **Config**: Configuration files.
  - `config.php`: Main configuration file.

- **Controllers**: Controllers that handle application logic.
  - `errors.php`: Error handling controller.
  - `home.php`: Home controller.

- **Helpers**: Helper functions.
  - `helpers.php`: Helper functions file.

- **Libraries**: Core libraries for the framework.
  - **Core**:
    - `Autoload.php`: Handles automatic class loading.
    - `Connection.php`: Database connection handling.
    - `Controllers.php`: Base controller class.
    - `Load.php`: Class for loading controllers, models, and views.
    - `Mysql.php`: MySQL database interaction class.
    - `Views.php`: View rendering class.

- **Models**: Data models.
  - `HomeModels.php`: Model for the home controller.

- **Views**: Views and templates.
  - **Errors**: Error view templates.
  - **Templates**:
    - `home.php`: Main home view template.

## Requirements

- PHP 7.4 or higher

## Installation

1. Clone the Repository:

   ```sh
   git clone https://github.com/davidrbh/mini_framework.git
   ```
2. Copy the project folder to your web server's root directory.
3. Access the application via your browser at http://localhost/mini_framework.


## Configuration

To set the root URL of your web application, modify the $url variable in the `index.php` file. By default, it is set to 'home/home'. Change this value to match the desired default route for your application.
  

**Example modification in index.php:**

   ```
   $url = $_GET['url'] ?? 'your-controller/your-method';
   ```

## Usage

1. Define Routes: In the routes file, map URLs to controllers and methods.

2. Create Controllers: Define controllers in the controllers folder and link them to the defined routes.

3. Create Views: Design views in the views folder to display the user interface.

4. Run the Application:
   - For production deployment, place the project folder in the root directory of your web server.
     
  
## Contributing

**Contributions are welcome. If you wish to improve the project, please follow these steps:**

1. Fork the repository.
2. Create a new branch (git checkout -b feature/new-feature).
3. Make changes and commit them (git commit -am 'Add new feature').
4. Push your changes and submit a pull request.

## License

This project is licensed under the MIT License.

## Author

Developed by davidrbh.



