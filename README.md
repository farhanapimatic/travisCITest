# Getting started

## How to Build

The generated code uses a few Maven dependencies e.g., Jackson, UniRest,
and Apache HttpClient. The reference to these dependencies is already
added in the pom.xml file will be installed automatically. Therefore,
you will need internet access for a successful build.

* In order to open the client library in Eclipse click on ``` File -> Import ```.

![Importing SDK into Eclipse - Step 1](https://apidocs.io/illustration/java?step=import0&workspaceFolder=Hello%20world%204-Java&workspaceName=HelloWorld4&projectName=HelloWorld4Lib&rootNamespace=com.example)

* In the import dialog, select ``` Existing Java Project ``` and click ``` Next ```.

![Importing SDK into Eclipse - Step 2](https://apidocs.io/illustration/java?step=import1&workspaceFolder=Hello%20world%204-Java&workspaceName=HelloWorld4&projectName=HelloWorld4Lib&rootNamespace=com.example)

* Browse to locate the folder containing the source code. Select the detected location of the project and click ``` Finish ```.

![Importing SDK into Eclipse - Step 3](https://apidocs.io/illustration/java?step=import2&workspaceFolder=Hello%20world%204-Java&workspaceName=HelloWorld4&projectName=HelloWorld4Lib&rootNamespace=com.example)

* Upon successful import, the project will be automatically built by Eclipse after automatically resolving the dependencies.

![Importing SDK into Eclipse - Step 4](https://apidocs.io/illustration/java?step=import3&workspaceFolder=Hello%20world%204-Java&workspaceName=HelloWorld4&projectName=HelloWorld4Lib&rootNamespace=com.example)

## How to Use

The following section explains how to use the HelloWorld4 library in a new console project.

### 1. Starting a new project

For starting a new project, click the menu command ``` File > New > Project ```.

![Add a new project in Eclipse](https://apidocs.io/illustration/java?step=createNewProject0&workspaceFolder=Hello%20world%204-Java&workspaceName=HelloWorld4&projectName=HelloWorld4Lib&rootNamespace=com.example)

Next, choose ``` Maven > Maven Project ```and click ``` Next ```.

![Create a new Maven Project - Step 1](https://apidocs.io/illustration/java?step=createNewProject1&workspaceFolder=Hello%20world%204-Java&workspaceName=HelloWorld4&projectName=HelloWorld4Lib&rootNamespace=com.example)

Here, make sure to use the current workspace by choosing ``` Use default Workspace location ```, as shown in the picture below and click ``` Next ```.

![Create a new Maven Project - Step 2](https://apidocs.io/illustration/java?step=createNewProject2&workspaceFolder=Hello%20world%204-Java&workspaceName=HelloWorld4&projectName=HelloWorld4Lib&rootNamespace=com.example)

Following this, select the *quick start* project type to create a simple project with an existing class and a ``` main ``` method. To do this, choose ``` maven-archetype-quickstart ``` item from the list and click ``` Next ```.

![Create a new Maven Project - Step 3](https://apidocs.io/illustration/java?step=createNewProject3&workspaceFolder=Hello%20world%204-Java&workspaceName=HelloWorld4&projectName=HelloWorld4Lib&rootNamespace=com.example)

In the last step, provide a ``` Group Id ``` and ``` Artifact Id ``` as shown in the picture below and click ``` Finish ```.

![Create a new Maven Project - Step 4](https://apidocs.io/illustration/java?step=createNewProject4&workspaceFolder=Hello%20world%204-Java&workspaceName=HelloWorld4&projectName=HelloWorld4Lib&rootNamespace=com.example)

### 2. Add reference of the library project

The created Maven project manages its dependencies using its ``` pom.xml ``` file. In order to add a dependency on the *HelloWorld4Lib* client library, double click on the ``` pom.xml ``` file in the ``` Package Explorer ```. Opening the ``` pom.xml ``` file will render a graphical view on the cavas. Here, switch to the ``` Dependencies ``` tab and click the ``` Add ``` button as shown in the picture below.

![Adding dependency to the client library - Step 1](https://apidocs.io/illustration/java?step=testProject0&workspaceFolder=Hello%20world%204-Java&workspaceName=HelloWorld4&projectName=HelloWorld4Lib&rootNamespace=com.example)

Clicking the ``` Add ``` button will open a dialog where you need to specify HelloWorld4 in ``` Group Id ``` and HelloWorld4Lib in the ``` Artifact Id ``` fields. Once added click ``` OK ```. Save the ``` pom.xml ``` file.

![Adding dependency to the client library - Step 2](https://apidocs.io/illustration/java?step=testProject1&workspaceFolder=Hello%20world%204-Java&workspaceName=HelloWorld4&projectName=HelloWorld4Lib&rootNamespace=com.example)

### 3. Write sample code

Once the ``` SimpleConsoleApp ``` is created, a file named ``` App.java ``` will be visible in the *Package Explorer* with a ``` main ``` method. This is the entry point for the execution of the created project.
Here, you can add code to initialize the client library and instantiate a *Controller* class. Sample code to initialize the client library and using controller methods is given in the subsequent sections.

![Adding dependency to the client library - Step 2](https://apidocs.io/illustration/java?step=testProject2&workspaceFolder=Hello%20world%204-Java&workspaceName=HelloWorld4&projectName=HelloWorld4Lib&rootNamespace=com.example)

## How to Test

The generated code and the server can be tested using automatically generated test cases. 
JUnit is used as the testing framework and test runner.

In Eclipse, for running the tests do the following:

1. Select the project *HelloWorld4Lib* from the package explorer.
2. Select "Run -> Run as -> JUnit Test" or use "Alt + Shift + X" followed by "T" to run the Tests.

## Initialization

### 

API client can be initialized as following.

```java

HelloWorld4Client client = new HelloWorld4Client();
```


# Class Reference

## <a name="list_of_controllers"></a>List of Controllers

* [HelloworldController](#helloworld_controller)

## <a name="helloworld_controller"></a>![Class: ](https://apidocs.io/img/class.png "com.example.controllers.HelloworldController") HelloworldController

### Get singleton instance

The singleton instance of the ``` HelloworldController ``` class can be accessed from the API Client.

```java
HelloworldController helloworld = client.getHelloworld();
```

### <a name="get_helloworld_async"></a>![Method: ](https://apidocs.io/img/method.png "com.example.controllers.HelloworldController.getHelloworldAsync") getHelloworldAsync

> TODO: Add a method description


```java
void getHelloworldAsync(final APICallBack<HelloWorldResponse> callBack)
```

#### Example Usage

```java
// Invoking the API call with sample inputs
helloworld.getHelloworldAsync(new APICallBack<HelloWorldResponse>() {
    public void onSuccess(HttpContext context, HelloWorldResponse response) {
        // TODO success callback handler
    }
    public void onFailure(HttpContext context, Throwable error) {
        // TODO failure callback handler
    }
});

```


[Back to List of Controllers](#list_of_controllers)



