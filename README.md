# vigoCucumberJVM
CucumberJVM  middleware for https://vigoreport.io


### **Integration** with vigoreport.io
----------------------

>**Prerequisites**
    1. You need to to have the Java Development Kit (JDK) installed and available.
    2. You will also need to have Cucumber JVM Report Directory Path.
    3. You will also need Project Key For the configuration.


>**NOTE** : Please add this - "json:target/cucumber.json" into your  @cucumberoption
```
Eg.  @CucumberOptions(
        format = { 
          "html:target/cucumber-html-report",
          "pretty", "html:target1/cucumber",
          "json:target/cucumber.json" }, 
          features = { "path of feature file"
        })
```


####STEP-1
>Download the `Vigo-CucumberJVM-xxx.jar` from this repo.

####STEP-2.
>Generating Config file
`Java -jar VigoBot-CucumberJVM-xxx.jar -init`

####STEP-3.
>Add Report directoryPath and Project key into config file
```
{
    "projectKey":"502d97c9a94567GH59711966a3ec8d758",
    "reportDirectory":"F:/TestingProjectWorkspace/Test1/target"
}
```

####STEP-4.
>Start the VigoBot-CucumberJvm & Enjoy reporting on web.
 `Java -jar Vigo-CucumberJVM-xxx.jar`
 
####STEP-5
 After VigoBot is started, Execute your automation code to track the result.
