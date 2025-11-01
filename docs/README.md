import os

def get_project_info():
    """Returns project information as a dictionary."""
    project_info = {
        "name": "Frontend App",
        "description": "A frontend application developed using modern web technologies.",
        "version": "1.0.0",
        "author": "Your Name",
        "email": "your.email@example.com",
        "github": "https://github.com/your-username/frontend-app"
    }
    return project_info

def get_dependencies():
    """Returns a list of dependencies required to run the project."""
    dependencies = [
        "npm",
        "yarn",
        "typescript",
        "webpack",
        "react",
        "react-dom",
        "react-router-dom"
    ]
    return dependencies

def get_environment_variables():
    """Returns a dictionary of environment variables required to run the project."""
    env_variables = {
        "NODE_ENV": "development",
        "PORT": 3000,
        "DB_URI": "mongodb://localhost:27017"
    }
    return env_variables

def get_license():
    """Returns the license information for the project."""
    license_info = {
        "name": "MIT License",
        "url": "https://opensource.org/licenses/MIT"
    }
    return license_info

def main():
    """Main function that prints the project information."""
    print("Project Name:", get_project_info()["name"])
    print("Project Description:", get_project_info()["description"])
    print("Dependencies:")
    for dependency in get_dependencies():
        print(dependency)
    print("Environment Variables:")
    for variable, value in get_environment_variables().items():
        print(f"{variable}={value}")
    print("License:", get_license()["name"])
    print(get_license()["url"])

if __name__ == "__main__":
    main()