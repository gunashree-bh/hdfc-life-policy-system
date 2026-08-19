**HDFC Life Policy System**

This is a Java-based policy management system developed as part of the HDFC Life assessment. The project focuses on Java OOP concepts, Collections, SOLID principles, design patterns, exception handling, and file handling.

Features

Create and manage different types of policies

Search policies using policy number

Create and validate insurance claims

Handle claims based on urgency

Send notifications when claim status changes

Maintain an audit log for filed claims

**Technologies Used**

Java

IntelliJ IDEA

Java Collections Framework

Design Patterns Used

Singleton

AppConfig uses an enum-based Singleton to store application-level configuration such as the company name and maximum claim amount.

Factory

PolicyFactory creates the required policy object based on the policy type.

**Supported policy types:**

TERM

ULIP

ENDOWMENT

Builder

Claim.Builder is used to create claim objects with required and optional details.

Strategy

Premium calculation is handled using separate strategies for:

Term Life

ULIP

Endowment

The ULIP calculation for a premium of 42000 gives 47040.

Observer

The claim notification system uses the Observer pattern with:

InAppNotifier

BranchLetterNotifier

Both observers are notified when the claim status changes.

Collections Used

ArrayList – stores all policies

HashSet – keeps unique customer names

HashMap – searches policies using policy number

TreeMap – keeps policy numbers sorted

PriorityQueue – handles claims according to urgency

Exception Handling

Custom exceptions are used for:

Policy not found

Invalid claim amount

Unknown policy type

The application demonstrates all three cases in Main.java.

**Project Structure**

src/

└── com/hdfclife/

    ├── Main.java

    ├── config/

    ├── exception/

    ├── factory/

    ├── model/

    ├── observer/

    ├── service/

    ├── store/

    └── strategy/

**How to Run**

Open the project in IntelliJ IDEA.

Set the project SDK to Java 17 or above.

Open Main.java.

Run the main() method.

Check the console output.

The application creates an audit.log file when claims are filed.

Sample Results

Company -> HDFC Life

Unique customer count -> 5

Lookup HDFC-LIFE-1004 -> Vikram Singh

ULIP premium for HDFC-LIFE-1002 -> 47040

PriorityQueue poll order -> HIGH, MEDIUM, LOW

The application also demonstrates claim notifications and custom exception handling.

HDFC Life Policy System

This is a Java-based policy management system developed as part of the HDFC Life assessment. The project focuses on Java OOP concepts, Collections, SOLID principles, design patterns, exception handling, and file handling.

Features

* Create and manage different types of policies

* Search policies using policy number

* Create and validate insurance claims

* Handle claims based on urgency

* Send notifications when claim status changes

* Maintain an audit log for filed claims

Technologies Used

* Java

* IntelliJ IDEA

* Java Collections Framework

**Design Patterns Used**

Singleton

AppConfig uses an enum-based Singleton to store application-level configuration such as the company name and maximum claim amount.

Factory

PolicyFactory creates the required policy object based on the policy type.

Supported policy types:

* TERM

* ULIP

* ENDOWMENT

Builder

Claim.Builder is used to create claim objects with required and optional details.

Strategy

Premium calculation is handled using separate strategies for:

* Term Life

* ULIP

* Endowment

The ULIP calculation for a premium of 42000 gives 47040.

Observer

The claim notification system uses the Observer pattern with:

* InAppNotifier

* BranchLetterNotifier

Both observers are notified when the claim status changes.

Collections Used

* ArrayList – stores all policies

* HashSet – keeps unique customer names

* HashMap – searches policies using policy number

* TreeMap – keeps policy numbers sorted

* PriorityQueue – handles claims according to urgency

Exception Handling

Custom exceptions are used for:

* Policy not found

* Invalid claim amount

* Unknown policy type

The application demonstrates all three cases in Main.java.

Project Structure

src/

└── com/hdfclife/

    ├── Main.java

    ├── config/

    ├── exception/

    ├── factory/

    ├── model/

    ├── observer/

    ├── service/

    ├── store/

    └── strategy/

How to Run

1. Open the project in IntelliJ IDEA.

2. Set the project SDK to Java 17 or above.

3. Open Main.java.

4. Run the main() method.

5. Check the console output.

The application creates an audit.log file when claims are filed.

Sample Results

Company -> HDFC Life

Unique customer count -> 5

Lookup HDFC-LIFE-1004 -> Vikram Singh

ULIP premium for HDFC-LIFE-1002 -> 47040

PriorityQueue poll order -> HIGH, MEDIUM, LOW

The application also demonstrates claim notifications and custom exception handling.
 
