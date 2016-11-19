# json-postman
JSON Automation Test Case via Postman

## Abstract
### Why Validate Data as a Separate Step?
	* to fail fast
	* to avoid data corruption
	* to simplify processing code
	* to use validation code in tests
		
### Why JSON (and not XML)?
	* as wide adoption as XML
	* easier to process and more concise than XML
	* dominates web development because of JavaScript

### Why Use Schemas?
	* declarative
	* easier to maintain
	* can be understood by non-coders
	* no need to write code, third party open-source libraries can be used

### Why JSON-Schema?
	* the widest adoption among all standards for JSON validation
	* very mature (current version is 4, there are proposals for version 5)
	* covers a big part of validation scenarios
	* uses easy-to-parse JSON documents for schemas
	* platform independent
	* easily extensible
	* 30+ validators for different languages, including 10+ for JavaScript, so no need to code it yourself
	
### Why Using This Repo (zeroc0d3/json-postman)?
	* tested result
	* easy to learn from simple to complex condition
	* using schema references to validate the response
	* using external library PostmanBDD not only TinyValidator (tv4)

## Installation
1. Install postman.
2. Install tv4 (Tiny Validator).
   * npm install tv4
3. Install ajv (Another JSON Schema Validator).
   * npm install ajv
4. Copy & paste the testcase script on tab "test" postman.
5. Done.
	
## Runner Postman
1. Import the collection in folder "collection", or
2. Download ZeroC0D3 Collection :
   https://www.getpostman.com/collections/7f63ef54d405bfe2f1db
3. Click "Runner" button and select the "ZeroC0D3 TestCase API",
4. Click "Start Runner" button.
5. Done.

## Using Newman
1. Download test result "ZeroC0D3_Result.json" in folder "collection".
2. Install newman
   * npm install -g newman
3. Open your terminal / command,
4. Running newman command
   * newman -c ZeroC0D3_Result.json 	
5. Done.
   
## References
1. http://blog.getpostman.com/2014/03/07/writing-automated-tests-for-apis-using-postman/
2. http://blog.getpostman.com/2014/04/17/how-to-write-automated-tests-for-apis-with-postman-part-2/
3. https://github.com/geraintluff/tv4
4. http://geraintluff.github.com/tv4/
5. https://github.com/BigstickCarpet/postman-bdd
6. https://spacetelescope.github.io/understanding-json-schema/structuring.html
7. http://chaijs.com/plugins/chai-json-schema/
8. https://code.tutsplus.com/tutorials/validating-data-with-json-schema-part-1--cms-25343
9. https://code.tutsplus.com/tutorials/validating-data-with-json-schema-part-2--cms-25640
