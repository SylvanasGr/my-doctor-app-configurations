## Centralized Configuration with GitHub Project

This GitHub project serves as a centralized configuration repository for your microservices, streamlining the process of managing configurations across multiple services.

## How it Works

**Setting up Configuration for "TomatoProject"**

Imagine you have a microservice named "TomatoProject." Here's how you can leverage this configuration system to centralize your settings:

1. **Specify Project Name in `bootstrap.yml`:**

Start by specifying the name of your "TomatoProject" in the `bootstrap.yml` file of your microservice. Add the following line to the file:

        spring.application.name=tomato-project


2. **Create Configuration Folder:**

Create a folder with the same name as your project, which, in this case, is `tomato-project`.


3. **Add Configuration Files:**

Inside the newly created folder, you'll provide the corresponding configuration files. These files should follow a specific naming convention, where `application-profileyouwant` represents the specific profile you need. For example:

* `application.yml` for the default profile.
* `application-local.yml` for the local profile.
* `application-production.yml` for the production profile.

**Your folder structure should look like this:**

    tomato-project
    ├── application.yml
    ├── application-local.yml
    ├── application-production.yml
    └── ...


4. **Run the Application:**

Finally, run your microservice with the desired profile. This configuration approach ensures that your service picks up the appropriate settings based on the active profile, offering enhanced flexibility and readability for your microservice setup.

## Benefits of Centralized Configuration

By adopting this centralized configuration approach and adhering to these guidelines, you can effectively manage configuration settings across your microservices, promoting a more organized and maintainable system.

* **Improved visibility and control:** Centralizing your configurations in a single repository makes it easier to track and manage changes. You can also use Git features to ensure that changes are reviewed and approved before being deployed.
* **Reduced duplication:** Centralizing your configurations eliminates the need to duplicate the same settings in multiple places. This can save time and effort, and it also helps to ensure that your configurations are consistent across all of your microservices.
* **Simplified deployment:** Centralized configuration makes it easier to deploy new versions of your microservices. You simply need to update the configuration repository and then restart your microservices. This ensures that all of your microservices are using the same configuration, regardless of when they were deployed.

Overall, centralized configuration offers a number of benefits for microservices architectures. By following the guidelines above, you can implement centralized configuration effectively and efficiently.

