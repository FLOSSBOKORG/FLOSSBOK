# Testing

---

Testing is an important part of software engineering process. It helps to find out defects of your product before your users find them. Although technically it may not be feasible to find out all defects before your product releases, a more complete testing process help to lower the chance your users encounter issues. There are different types of testing. We will discuss some of them.

## Unit Testing

Unit testing is a level of software testing where individual units/ components of a software are tested. The purpose is to validate that each unit of the software performs as designed. A unit is the smallest testable part of software. It usually has one or a few inputs and usually a single output. Unit testing oftentimes is done through automation, but they can also be do manually. The objective in unit testing is to isolate a unit and validate its correctness. In open source projects, each contributor can write their own unite tests for the components he/she is responsible for. Usually a project owner chooses a testing framework and other create test cases on top of it. As a good practice, unit tests need to be done before sending pull requests.

## Integration Testing

Integration Testing is a level of software testing where individual units are combined and tested as a group. The purpose of this level of testing is to expose faults in the interaction between integrated units. When two or more units are ready, they are assembled and integration testing is performed. Unlike unit test focuses on the component itself, integration testing focuses more on the interaction between different components. A component works fine on its own cannot guarantee it will work with others as well.

## System Testing

System testing of software or hardware is testing conducted on a complete, integrated system to evaluate the system's compliance with its specified requirements. It is also intended to test up to and beyond the bounds defined in the software/hardware requirements specification. It is a part of black-box testing. There are many tests can be done in this areas, such as usability testing, load/stress testing, accessibility testing, performance testing, etc. Since this area include many tests that requires different expertise, in open source projects, the project owner can recruit volunteers from the public and assign testing tasks based on skill sets.

## Acceptance Testing

Acceptance Testing is a level of the software testing where a system is tested for acceptability. The purpose of this test is to evaluate the system’s compliance with the business requirements and assess whether it is acceptable for delivery. Like system testing, acceptance testing is within the scope of black-box testing. The project owners check if the project meets acceptance criteria. Usually the process is not scripted and is rather ad-hoc. Based on experience the project owners can know if the current state of the project is mature enough so that they could bump up the version.

