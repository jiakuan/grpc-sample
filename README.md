This is a sample project for using gRPC in Java and Gradle.

This project was created based on [https://github.com/grpc/grpc-java/tree/master/examples](https://github.com/grpc/grpc-java/tree/master/examples). The purpose of this project is to arrange it in a separate project, which then can be used as a template.

You can use it as a template project when starting a new project.

Before importing into your IDE, please build the project from command line first, so that it can generate code from proto files.

To build, please run the command below:

	gradle clean build

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

After build, the proto Java classes will be generated under `src/generated` folder.


## Sponsor

If you would like to contribute this project, please feel free to fork and create pull requests, or contact us at: support (at) wisepersist dot com

This project is sponsored by: [TaskTips](https://task.tips).
