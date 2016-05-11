This is a sample project for using gRPC in Java and Gradle.

This project was created based on [https://github.com/grpc/grpc-java/tree/master/examples](https://github.com/grpc/grpc-java/tree/master/examples). The purpose of this project is to arrange it in a separate project, which then can be used as a template.

You can use it as a template project when starting a new project.

To build, please run the command below:

	gradle clean build

After build, the proto Java classes will be generated under `src/generated` folder.

If you see issues like this:

```
FAILURE: Build failed with an exception.

* Where:
Build file '.../grpc-sample/build.gradle' line: 3

* What went wrong:
A problem occurred evaluating root project 'grpc-sample'.
> Failed to apply plugin [id 'com.google.protobuf']
   > Could not create an instance of type com.google.protobuf.gradle.ProtobufSourceDirectorySet_Decorated.

* Try:
Run with --stacktrace option to get the stack trace. Run with --info or --debug option to get more log output.

BUILD FAILED

Total time: 53.602 secs
```

You may need to downgrade your Gradle to 2.10.