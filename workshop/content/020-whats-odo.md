OpenShift Do (odo) is a CLI tool for developers who are writing, building, and deploying applications on OpenShift. With odo, developers get an opinionated CLI tool that supports fast, iterative development. Odo abstracts away Kubernetes and OpenShift concepts so developers can focus on what's most important to them: __code__.

Odo was created to improve the developer experience with OpenShift. Existing tools such as `oc` are more operations-focused and require a deep understanding of Kubernetes and OpenShift concepts. Odo is designed to be __simple__ and __concise__ so you can focus on coding rather than how to deploy your application. Since odo can build and deploy your code to your cluster immediately after you save your changes, you benefit from instant feedback and can validate your changes in real-time. Odo's syntax and design is centered around concepts already familiar to developers, such as project, application, and component.

## Features

- Designed for fast, iterative development cycles
- 100% client based. No server required within your OpenShift cluster for deployment
- Supports multiple languages and frameworks such as Node.js, Java, Ruby, Perl, PHP and Python
- Detect changes to your local code and deploy automatically with `odo watch`
- List all available components and services from your OpenShift cluster

## Glossary
In odo there are some terms that people often times use for different purposes. That's why we need to define them here for common understanding moving forward:

- __Component__: A constituent part of an application that is where your business logic resides, such as user-facing front ends or server-side backends. A component may have different attributes like storage, configuration, urls, etc. Multiple component types are currently supported, like Node.js, Perl, PHP, Python, Ruby, etc.
- __Service__: A service is typically a dependency that a component links to and depends on, but that has no business logic in it. For example: MariaDB, Jenkins, or Redis. These come from the OpenShift "Service Catalog" that must be enabled within your cluster.
- __Application__: An application represents, no surprise, the application you are creating. An application serves as a loose grouping concept to group the components and services together. A complex application, for example, may consist of multiple components and services working collaboratively to provide the full business value.