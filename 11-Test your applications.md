# Sheet n°11: Test your applications

#### Testing your product allows you to check its correct operation, to ensure a good user experience and to find and prevent defects before it goes into production. Testing your product also reduces the risk of personal data breaches.

## Automate testing

* The **development tests** (unit, functional, etc.) will verify the adequacy between the specifications and the functioning of the product. The **security tests** (random data tests also called "_fuzzing_", _scan_ of vulnerabilities, etc.), will check that the product continues to function acceptably when you move away from its normal use and that it does not present any vulnerability that could allow third parties to compromise its security. Both types of tests are important for the proper functioning of your application.

* Set up a **continuous integration system** to run the tests automatically after each change in your source code.

## Integrate testing into your business strategy.

* Add the implementation of the test environment into the company's strategy. The **acceptable metrics** must be defined jointly by all parties prior to development.

* Metrics to consider are for example:

    * The **coverage rate** of tests and their type;
    * the **duplication rate** of your code;
    * the **number of vulnerabilities** (as defined by the tools) and their type, etc.

## Watch out for your test data!

* "Real" production data should not be used during the development and testing phase. Using personal data from your production database for testing purposes is tantamount to **diverting it from its original purpose**.

* If personal data is used outside of production, it should be noted that the **security risks** are also **increased**: access to the data by people who do not have a need to know, multiple storage locations, etc.

* So build a **dummy data set** that will look like the data that will be processed by your application. A dummy data set will ensure that disclosure of this data will not have any impact on people.

* If you need to **import existing configurations** from production into your test cases, consider **anonymizing the personal data** that may be present.
