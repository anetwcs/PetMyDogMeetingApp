# PetMyDog

Developer Guide: https://github.com/anetwcs/PetMyDogMeetingApp/blob/main/docs/dev_guide.md

User Manual: https://github.com/anetwcs/PetMyDogMeetingApp/blob/main/docs/user_guide.md

[![MIT License](https://img.shields.io/apm/l/atomic-design-ui.svg?)](https://github.com/tterb/atomic-design-ui/blob/master/LICENSEs)<br><br>
[User Document](https://github.com/evaliu2002/PetMyDog/blob/main/USERDOC.md)

<img width="286" alt="image" src="https://user-images.githubusercontent.com/69877857/171104547-4c8e61b5-257b-4838-bbc4-c735bddec6d9.PNG">
<img width="286" alt="image" src="https://user-images.githubusercontent.com/69877857/171105202-cd21a465-2767-4a76-8397-03ea645b03b7.png">
<img width="286" alt="image" src="https://user-images.githubusercontent.com/69877857/171105293-5868d950-7ed6-4a0f-aa55-4966d5c8f26b.png">
<img width="286" alt="image" src="https://user-images.githubusercontent.com/69877857/171105327-84ee1e8a-1165-4389-999e-7a38820c689f.png">
<img width="286" alt="image" src="https://user-images.githubusercontent.com/69877857/171105358-3053eef5-5704-4eb1-829f-11f2e18bde53.png">
<img width="286" alt="image" src="https://user-images.githubusercontent.com/69877857/171105403-42cef8e7-d64d-4a4e-bdad-aab0b13fe540.png">
<img width="286" alt="image" src="https://user-images.githubusercontent.com/69877857/171104698-2a12273c-5b10-4e44-8c48-2dd6bfa0937e.PNG">
<img width="284" alt="image" src="https://user-images.githubusercontent.com/69877857/171104766-57fa4d67-5c10-4d2f-b08f-e33c1fc3a8b3.PNG">
<img width="284" alt="image" src="https://user-images.githubusercontent.com/69877857/171104868-a3817d9c-e584-4217-a99e-fa68272f3ff1.PNG">
<img width="286" alt="image" src="https://user-images.githubusercontent.com/69877857/171105059-f786474f-80b0-4a74-b716-97812f2545fa.png">
<img width="286" alt="image" src="https://user-images.githubusercontent.com/69877857/171105565-d66b244b-814e-40da-98a3-8c7a693c5dcc.png">
<img width="286" alt="image" src="https://user-images.githubusercontent.com/69877857/171105729-ea7856e9-0b8f-4b9a-afdb-d53f59656f00.PNG">
<img width="286" alt="image" src="https://user-images.githubusercontent.com/69877857/171105744-cc016aac-b4c7-4c13-bac3-d54eefe5831a.PNG">

### Project Idea/Goal

Pet My Dog will be a web app that allows dog owners to broadcast their location while
walking their dogs, during which other nearby users of the app can locate owners in real time
and follow them to pet their dogs. In addition to broadcasting their location, owners can also
share small amounts of information about themselves and their dogs to nearby users.

Some main features we will implement include user registration, dog profiles, retrieving nearby
pets in map and list view, requesting and accepting meetups with nearby dogs, and searching for
pets by name. Some stretch goals we could implement include calling and messaging between users,
invitation system for meetups, a like system for owners and petters for safety precautions, filtering
system, and redirection to other social media platforms (e.g., instagram, facebook).

### Operational Use Case(s)

The user can now login/sign up using Google Login. Once the user logs in/signs up, the user is redirected
back to the login/sign up page where they can press the button to redirect their page to the find dogs
page. The find dogs page displays a map with a marker of the user's current location, a 500 meter circle
around the user's marker, and lists all the nearby dogs within 500 meters of the user's location. The 
user can press the dog and is redirected to the selected dog page where information about the dog is displayed.

### Layout of the repository

All the code will be contained in the main directory. The main directory is divided into front
and back end code, each in a sub directory. We will have our weekly reports in the Weekly Reports
directory, which we will update every week to report our progress and action items. Our tests are contained
within the front and back end sub directories, within the src sub directory (and the tests are in the test
sub directory).

### Building a release of the software

Pushing to the main branch will automatically build the software, so there is no manual intervention needed.

## Back-end:

### Setup Instructions (for use in IntelliJ with Maven):

#### Building and Running the project
1. Build the project in IntelliJ by navigating to the Maven tab in IntelliJ, opening `Lifecycle` in the `back-end` tab, and clicking the
   `Compile` button.
2. Run Elasticsearch locally. Follow the instructions provided here:
   https://www.elastic.co/downloads/elasticsearch
3. Run `Main.java` to launch the Spark server on localhost port 4567.

#### Testing the project
1. Run Elasticsearch locally before testing by following the instructions provided here:
   https://www.elastic.co/downloads/elasticsearch
2. Navigate to the Maven tab in IntelliJ, open `Lifecycle` in the `back-end` tab, and click the `Test` button to run the provided
   tests.
3. JUnit tests are located and can be added in main/back-end/src/test/java.
4. Before running JUnit tests, make sure that Main.java is not running already. Otherwise, stop Main.java.

#### Adding new tests

To add a new test, navigate to `main/back-end/src/test`, and add the test to the appropriate test file.

For naming conventions, we name the test based on the use case it will be testing. Each test should go into the corresponding
Java test file for the method it is testing (ex: for testing getUserProfile in Main.java, we add our test to GetUserProfileTest.java).

## Front-end:

### Setup Instructions

1. Obtain source code by cloning this repo.

2. Navigate to main/front-end.

3. Run npm install.
4. Users will also be
   prompted by IntelliJ or npm to install all the imported
   packages used for the project. Users may proceed to install
   the imported packages.

5. To run PetMyDog on localhost, run npm start.

#### How to run tests
1. Navigate to main/front-end.
2. Run npm test.

#### Adding new tests

To add a new test, navigate to `main/front-end/src/test`, and add the test to the appropriate test file.

#### How to build a release of the software
1. Navigate to main/front-end.
2. Run npm build.

## How to file a Bug Report:
To report a bug, navigate to our [Issue](https://github.com/evaliu2002/PetMyDog/issues/new/choose) page nad choose the
Bug Report template and fill in the information below:
- Describe the bug: A clear and concise description of what the bug is.
- To Reproduce: Steps to reproduce the behavior.
- Expected behavior: A clear and concise description of what you expected to happen.
- Screenshots: If applicable, add screenshots to help explain your problem.
- Desktop: Information regarding your PC, if applicable.
- Smartphone: Information regarding your phone, if applicable.
- Additional context: Add any other context about the problem here.
