
# pull a base image which gives all required tools and libraries
FROM openjdk:17-jdk-alpine

#create a directory where the app code will be stored
WORKDIR /app

#Copy the source code from your Host machine to container
COPY src/Main.java /app/Main.java

#Compile the app code
RUN javac Main.java

#run the application and by below command additional 

CMD ["java","Main"]
