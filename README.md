This is a sample project for using gRPC in Java and Gradle.

This project was created based on [https://github.com/grpc/grpc-java/tree/master/examples](https://github.com/grpc/grpc-java/tree/master/examples). The purpose of this project is to arrange it in a separate project, which then can be used as a template.

You can use it as a template project when starting a new project.

To build, please run the command below:

	gradle clean build

After build, the proto Java classes will be generated under `src/generated` folder.