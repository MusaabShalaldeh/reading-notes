# Configuring Django Settings

### What are the common issues when managing Django settings:


- Different environments. Usually, you have several environments: local, dev, ci, qa, staging, production, etc. Each environment can have its own specific settings (for example: DEBUG = True, more verbose logging, additional apps, some mocked data, etc). You need an approach that allows you to keep all these Django setting configurations.

- Sensitive data. You have SECRET_KEY in each Django project. On top of this there can be DB passwords and tokens for third-party APIs like Amazon or Twitter. This data cannot be stored in VCS.

- Sharing settings between team members. You need a general approach to eliminate human error when working with the settings. For example, a developer may add a third-party app or some API integration and fail to add specific settings. On large (or even mid-size) projects, this can cause real issues.

- Django settings are a Python code. This is a curse and a blessing at the same time. It gives you a lot of flexibility, but can also be a problem – instead of key-value pairs, settings.py can have a very tricky logic.


### Setting Configuration Approaches:

- **settings_local.py**

settings.py file:


**Pros:**
Secrets not in VCS.
**Cons:**
settings_local.py is not in VCS, so you can lose some of your Django environment settings.
The Django settings file is a Python code, so settings_local.py can have some non-obvious logic.
You need to have settings_local.example (in VCS) to share the default configurations for developers.

- **Separate settings file for each environment**

**Pros:**
All environments are in VCS.
It’s easy to share settings between developers.
**Cons:**
You need to find a way to handle secret passwords and tokens.
“Inheritance” of settings can be hard to trace and maintain.

- **Environment variables**

**Pros:**
Configuration is separated from code.
Environment parity – you have the same code for all environments.
No inheritance in settings, and cleaner and more consistent code.
There is a theoretical grounding for using environment variables – 12 Factors.
**Cons:**
You need to handle sharing default config between developers.

### What are the best pratices ?

* Keep settings in environment variables.
* Write default values for production configuration (excluding secret keys and tokens).
* Don’t hardcode sensitive settings, and don’t put them in VCS.
* Split settings into groups: Django, third-party, project.
* Follow naming conventions for custom (project) settings.


# SSH

### What is SSH? 

- SSH, or Secure Shell, is a remote administration protocol that allows users to control and modify their remote servers over the Internet. The service was created as a secure replacement for the unencrypted Telnet and uses cryptographic techniques to ensure that all communication to and from the remote server happens in an encrypted manner. It provides a mechanism for authenticating a remote user, transferring inputs from the client to the host, and relaying the output back to the client.


### How Does SSH Work?

- The SSH command consists of 3 distinct parts:

```bash
ssh {user}@{host}
```
The SSH key command instructs your system that you want to open an encrypted Secure Shell Connection. {user} represents the account you want to access. For example, you may want to access the root user, which is basically synonymous for system administrator with complete rights to modify anything on the system. {host} refers to the computer you want to access. This can be an IP Address (e.g. 244.235.23.19) or a domain name (e.g. www.xyzdomain.com).

When you hit enter, you will be prompted to enter the password for the requested account. When you type it in, nothing will appear on the screen, but your password is, in fact being transmitted. Once you’re done typing, hit enter once again. If your password is correct, you will be greeted with a remote terminal window.

### what are the three different encryption technologies used by SSH?

1. Symmetrical encryption.
2. Asymmetrical encryption.
3. Hashing.

### How Does SSH Work with These Encryption Techniques?

- The way SSH works is by making use of a client-server model to allow for authentication of two remote systems and encryption of the data that passes between them.

SSH operates on TCP port 22 by default (though this can be changed if needed). The host (server) listens on port 22 (or any other SSH assigned port) for incoming connections. It organizes the secure connection by authenticating the client and opening the correct shell environment if the verification is successful.


[Go Back](https://musaabshalaldeh.github.io/reading-notes/)