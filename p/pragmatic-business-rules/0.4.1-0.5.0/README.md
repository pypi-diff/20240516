# Comparing `tmp/pragmatic_business_rules-0.4.1.tar.gz` & `tmp/pragmatic_business_rules-0.5.0.tar.gz`

## Comparing `pragmatic_business_rules-0.4.1.tar` & `pragmatic_business_rules-0.5.0.tar`

### file list

```diff
@@ -1,22 +1,21 @@
--rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 pragmatic_business_rules-0.4.1/dev_requirements.txt
--rw-r--r--   0        0        0      471 2020-02-02 00:00:00.000000 pragmatic_business_rules-0.4.1/dprint.json
--rw-r--r--   0        0        0      129 2020-02-02 00:00:00.000000 pragmatic_business_rules-0.4.1/mypy.ini
--rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 pragmatic_business_rules-0.4.1/requirements.txt
--rw-r--r--   0        0        0     3869 2020-02-02 00:00:00.000000 pragmatic_business_rules-0.4.1/examples/long.json
--rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 pragmatic_business_rules-0.4.1/src/pragmatic_business_rules/__init__.py
--rw-r--r--   0        0        0     1211 2020-02-02 00:00:00.000000 pragmatic_business_rules-0.4.1/src/pragmatic_business_rules/action.py
--rw-r--r--   0        0        0     1244 2020-02-02 00:00:00.000000 pragmatic_business_rules-0.4.1/src/pragmatic_business_rules/asserts.py
--rw-r--r--   0        0        0     5533 2020-02-02 00:00:00.000000 pragmatic_business_rules-0.4.1/src/pragmatic_business_rules/condition.py
--rw-r--r--   0        0        0     2310 2020-02-02 00:00:00.000000 pragmatic_business_rules-0.4.1/src/pragmatic_business_rules/main.py
--rw-r--r--   0        0        0      670 2020-02-02 00:00:00.000000 pragmatic_business_rules-0.4.1/src/pragmatic_business_rules/types.py
--rw-r--r--   0        0        0     2895 2020-02-02 00:00:00.000000 pragmatic_business_rules-0.4.1/src/pragmatic_business_rules/validators.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pragmatic_business_rules-0.4.1/tests/__init__.py
--rw-r--r--   0        0        0     1369 2020-02-02 00:00:00.000000 pragmatic_business_rules-0.4.1/tests/test_action.py
--rw-r--r--   0        0        0    18526 2020-02-02 00:00:00.000000 pragmatic_business_rules-0.4.1/tests/test_condition.py
--rw-r--r--   0        0        0     6886 2020-02-02 00:00:00.000000 pragmatic_business_rules-0.4.1/tests/test_main.py
--rw-r--r--   0        0        0     1984 2020-02-02 00:00:00.000000 pragmatic_business_rules-0.4.1/tests/test_validators.py
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 pragmatic_business_rules-0.4.1/.gitignore
--rw-r--r--   0        0        0     1078 2020-02-02 00:00:00.000000 pragmatic_business_rules-0.4.1/LICENSE
--rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 pragmatic_business_rules-0.4.1/README.md
--rw-r--r--   0        0        0      761 2020-02-02 00:00:00.000000 pragmatic_business_rules-0.4.1/pyproject.toml
--rw-r--r--   0        0        0      733 2020-02-02 00:00:00.000000 pragmatic_business_rules-0.4.1/PKG-INFO
+-rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 pragmatic_business_rules-0.5.0/dev_requirements.txt
+-rw-r--r--   0        0        0      129 2020-02-02 00:00:00.000000 pragmatic_business_rules-0.5.0/mypy.ini
+-rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 pragmatic_business_rules-0.5.0/requirements.txt
+-rw-r--r--   0        0        0     3869 2020-02-02 00:00:00.000000 pragmatic_business_rules-0.5.0/examples/long.json
+-rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 pragmatic_business_rules-0.5.0/src/pragmatic_business_rules/__init__.py
+-rw-r--r--   0        0        0     1188 2020-02-02 00:00:00.000000 pragmatic_business_rules-0.5.0/src/pragmatic_business_rules/action.py
+-rw-r--r--   0        0        0     1607 2020-02-02 00:00:00.000000 pragmatic_business_rules-0.5.0/src/pragmatic_business_rules/asserts.py
+-rw-r--r--   0        0        0     5872 2020-02-02 00:00:00.000000 pragmatic_business_rules-0.5.0/src/pragmatic_business_rules/condition.py
+-rw-r--r--   0        0        0     2281 2020-02-02 00:00:00.000000 pragmatic_business_rules-0.5.0/src/pragmatic_business_rules/main.py
+-rw-r--r--   0        0        0      721 2020-02-02 00:00:00.000000 pragmatic_business_rules-0.5.0/src/pragmatic_business_rules/types.py
+-rw-r--r--   0        0        0     3489 2020-02-02 00:00:00.000000 pragmatic_business_rules-0.5.0/src/pragmatic_business_rules/validators.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pragmatic_business_rules-0.5.0/tests/__init__.py
+-rw-r--r--   0        0        0     1369 2020-02-02 00:00:00.000000 pragmatic_business_rules-0.5.0/tests/test_action.py
+-rw-r--r--   0        0        0    18470 2020-02-02 00:00:00.000000 pragmatic_business_rules-0.5.0/tests/test_condition.py
+-rw-r--r--   0        0        0     7902 2020-02-02 00:00:00.000000 pragmatic_business_rules-0.5.0/tests/test_main.py
+-rw-r--r--   0        0        0     1907 2020-02-02 00:00:00.000000 pragmatic_business_rules-0.5.0/tests/test_validators.py
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 pragmatic_business_rules-0.5.0/.gitignore
+-rw-r--r--   0        0        0     1078 2020-02-02 00:00:00.000000 pragmatic_business_rules-0.5.0/LICENSE
+-rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 pragmatic_business_rules-0.5.0/README.md
+-rw-r--r--   0        0        0      879 2020-02-02 00:00:00.000000 pragmatic_business_rules-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0      733 2020-02-02 00:00:00.000000 pragmatic_business_rules-0.5.0/PKG-INFO
```

### Comparing `pragmatic_business_rules-0.4.1/examples/long.json` & `pragmatic_business_rules-0.5.0/examples/long.json`

 * *Files identical despite different names*

### Comparing `pragmatic_business_rules-0.4.1/src/pragmatic_business_rules/action.py` & `pragmatic_business_rules-0.5.0/src/pragmatic_business_rules/action.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,47 +1,41 @@
 from .asserts import assert_comparable_type
-from .types import Action, number
+from .types import Action, Number
 from typing import Union
 
 
 # TODO
 # Move type validation of actions to the top level to exit early
 def apply_action_to_item(
 	action: Action,
 	item: str,
-	value: Union[number, str],
-) -> Union[number, str]:
+	value: Union[Number, str],
+) -> Union[Number, str]:
 	if len(action.keys()) > 1:
-		raise Exception(
-			"Too many actions '{}' were specified".format(", ".join(action.keys()))
-		)
+		raise Exception("Too many actions '{}' were specified".format(", ".join(action.keys())))
 
 	set = action.get("set")
 
 	# Specyfing set will replace the current value with the one passed to set
 	if set is not None:
 		try:
 			assert_comparable_type(item, value, None, set)
 		except Exception as e:
 			raise Exception(f"'set' action type differs from variable type: {str(e)}")
 
 		return set
 	else:
-		raise Exception(
-			"Unexpected '{}' action was specified".format(list(action.keys())[0])
-		)
+		raise Exception("Unexpected '{}' action was specified".format(list(action.keys())[0]))
 
 
 def apply_actions_to_variables(
 	actions: dict[str, Action],
-	variables: dict[str, Union[number, str]],
+	variables: dict[str, Union[Number, str]],
 ):
 	"""
 	This function mutates the variables object passed to it
 	"""
 	for item in actions:
 		if variables.get(item) is None:
-			raise Exception(
-				f"The key '{item}' is not defined in the variables object"
-			)
+			raise Exception(f"The key '{item}' is not defined in the variables object")
 
 		variables[item] = apply_action_to_item(actions[item], item, variables[item])
```

### Comparing `pragmatic_business_rules-0.4.1/src/pragmatic_business_rules/asserts.py` & `pragmatic_business_rules-0.5.0/src/pragmatic_business_rules/asserts.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,47 +1,53 @@
-from .types import Conditional
+from .types import Conditional, Operator
 from decimal import Decimal
 from typing import Any, Optional
 
+
 def assert_single_conditional(conditional: Conditional):
 	all = conditional.get("all")
 	any = conditional.get("any")
 
 	if all is not None and any is not None:
-		raise Exception(
-			"'all' and 'any' properties can't be specified for the same conditional"
-		)
+		raise Exception("'all' and 'any' properties can't be specified for the same conditional")
 	elif all is None and any is None:
-		raise Exception(
-			"'all' or 'any' properties were not found in the conditional"
-		)
+		raise Exception("'all' or 'any' properties were not found in the conditional")
 
 
 def assert_comparable_type(
 	label_1: Optional[str],
 	value_1: Any,
 	label_2: Optional[str],
 	value_2: Any,
 ):
+	if type(value_1) == list or type(value_2) == list:
+		if type(value_1) == list and type(value_2) == list:
+			raise Exception(
+				'Can\'t compare between two list values ({}"{}") and ({}"{}")'.format(
+					f'"{label_1}", ' if label_1 is not None else "",
+					value_1,
+					f'"{label_2}", ' if label_2 is not None else "",
+					value_2,
+				)
+			)
+		else:
+			return
+
 	# None is comparable to string and None
-	if (value_1 is None and value_2 is None) or (
-		type(value_1) == str and value_2 is None
-	) or (
-		value_1 is None and type(value_2) == str
-	):
+	if (value_1 is None and value_2 is None) or (type(value_1) == str and
+													value_2 is None) or (value_1 is None and type(value_2) == str):
 		return
 
 	# Decimal, ints and floats are comparable
 	if type(value_1) in [Decimal, int, float] and type(value_2) in [Decimal, int, float]:
 		return
 
 	if type(value_1) != type(value_2):
 		raise Exception(
-			'Can\'t compare values ({}"{}", {}) and ({}"{}", {})'
-			.format(
+			'Can\'t compare values ({}"{}", {}) and ({}"{}", {})'.format(
 				f'"{label_1}", ' if label_1 is not None else "",
 				value_1,
 				type(value_1).__name__,
 				f'"{label_2}", ' if label_2 is not None else "",
 				value_2,
 				type(value_2).__name__,
 			)
```

### Comparing `pragmatic_business_rules-0.4.1/src/pragmatic_business_rules/condition.py` & `pragmatic_business_rules-0.5.0/src/pragmatic_business_rules/condition.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,133 +1,137 @@
 from .asserts import assert_comparable_type, assert_single_conditional
-from .types import Condition, Conditional, number
+from .types import Condition, Conditional, Number
 from decimal import Decimal
 from typing import TypedDict, cast, Literal, Optional, Union
 
+
 class ConditionValues(TypedDict):
 	label_1: Optional[str]
 	label_2: Optional[str]
-	value_1: Union[None, number, str]
-	value_2: Union[None, number, str]
+	value_1: Union[None, Number, str]
+	value_2: Union[None, Number, str]
+
 
 def __get_condition_values(
 	condition: Condition,
-	constants: dict[str, Union[number, str]],
-	variables: dict[str, Union[number, str]],
+	constants: dict[str, Union[Number, str]],
+	variables: dict[str, Union[Number, str]],
 ) -> ConditionValues:
 	categories = list(filter(lambda k: k != "operator", condition.keys()))
 
 	if len(categories) == 0:
 		raise Exception("No values were found to execute the condition")
 	elif len(categories) != 2:
-		raise Exception(f'A condition must be composed by two categories of values, {"only " if len(categories) == 1 else ""}"{", ".join(sorted(categories))}" found')
-	
+		raise Exception(
+			f'A condition must be composed by two categories of values, {"only " if len(categories) == 1 else ""}"{", ".join(sorted(categories))}" found'
+		)
+
 	values: dict = {}
 	i = 1
 	for category in categories:
 		label: Optional[str] = None
-		value: Union[None, number, str]
+		value: Union[None, Number, list[Number], str, list[str]]
 
 		if category == "constant":
 			constant_name = cast(str, condition.get(category))
 			if constant_name not in constants:
 				raise Exception(f"Constant '{constant_name}' not defined")
 
 			label = constant_name
 			value = constants[constant_name]
 		elif category == "value":
 			value = condition[cast(Literal["value"], category)]
 		elif category == "variable":
 			variable_name = cast(str, condition.get(category))
 			if variable_name not in variables:
 				raise Exception(f"Variable '{variable_name}' not defined")
-			
+
 			label = variable_name
 			value = variables[variable_name]
 
 		if i == 1:
 			values["label_1"] = label
 			values["value_1"] = value
 		else:
 			values["label_2"] = label
 			values["value_2"] = value
 
 		i += 1
-	
+
 	return cast(ConditionValues, values)
 
+
 # By this point, the incoming conditions and variables have to have been already validated
 # for correct value types
 def evaluate_condition(
 	condition: Condition,
-	constants: dict[str, Union[number, str]],
-	variables: dict[str, Union[number, str]],
+	constants: dict[str, Union[Number, str]],
+	variables: dict[str, Union[Number, str]],
 ) -> bool:
 	condition_operator = condition["operator"]
 	values = __get_condition_values(condition, constants, variables)
 	value_1 = values["value_1"]
 	value_2 = values["value_2"]
 
 	assert_comparable_type(
 		values["label_1"],
 		value_1,
 		values["label_2"],
 		value_2,
 	)
 
+	if type(value_1) == list or type(value_2) == list:
+		if condition_operator == "in":
+			(haystack, needle) = (value_1, value_2) if type(value_1) == list else (value_2, value_1)
+			return needle in haystack  # type: ignore[operator]
+		else:
+			raise Exception(f"The operator '{condition_operator}' is not valid for list operations")
 	# The only value comparable to None is string, so they can be grouped in the same category
-	if type(value_1) == str or value_1 is None:
+	elif type(value_1) == str or value_1 is None:
 		if condition_operator == "equal_to":
 			return value_1 == value_2
 		else:
-			raise Exception(
-				f"The operator '{condition_operator}' is not valid for string operations"
-			)
+			raise Exception(f"The operator '{condition_operator}' is not valid for string operations")
 	elif type(value_1) == Decimal or type(value_1) == int or type(value_1) == float:
 		if condition_operator == "equal_to":
 			return value_1 == value_2
 		elif condition_operator == "greater_than_or_equal_to":
-			return value_1 >= value_2 # type: ignore[operator]
+			return value_1 >= value_2  # type: ignore[operator]
 		elif condition_operator == "greater_than":
-			return value_1 > value_2 # type: ignore[operator]
+			return value_1 > value_2  # type: ignore[operator]
 		elif condition_operator == "less_than_or_equal_to":
-			return value_1 <= value_2 # type: ignore[operator]
+			return value_1 <= value_2  # type: ignore[operator]
 		elif condition_operator == "less_than":
-			return value_1 < value_2 # type: ignore[operator]
+			return value_1 < value_2  # type: ignore[operator]
 		else:
-			raise Exception(
-				f"The operator '{condition_operator}' is not valid for number operations"
-			)
+			raise Exception(f"The operator '{condition_operator}' is not valid for number operations")
 	else:
 		raise Exception(
-			"The value '{}' has a type '{}' which is not valid for a condition value"
-			.format(
+			"The value '{}' has a type '{}' which is not valid for a condition value".format(
 				value_1,
 				type(value_1).__name__,
 			)
 		)
 
 
 def evaluate_conditional(
 	conditional: Optional[list[Union[Conditional, Condition]]],
-	constants: dict[str, Union[str, number]],
-	variables: dict[str, Union[str, number]],
+	constants: dict[str, Union[str, Number]],
+	variables: dict[str, Union[str, Number]],
 	type: Literal["all", "any"],
 ) -> bool:
 	"""
 	This function will evaluate the conditionals and return the boolean result for the entire group
 
 	The evaluation process is different depending on the type:
 	- all: All conditionals must be true
 	- any: At least one conditional must be true
 	"""
 	if type not in ["all", "any"]:
-		raise Exception(
-			f"The evaluation type '{type}' is not a valid conditional type"
-		)
+		raise Exception(f"The evaluation type '{type}' is not a valid conditional type")
 
 	if conditional is None:
 		return False
 
 	# Make sure that the conditional contains items that can be evaluated
 	# If no items were evaluated, mark the conditional as false
 	evaluated_items = 0
```

### Comparing `pragmatic_business_rules-0.4.1/src/pragmatic_business_rules/main.py` & `pragmatic_business_rules-0.5.0/src/pragmatic_business_rules/main.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from .action import apply_actions_to_variables
 from .asserts import assert_single_conditional
 from .condition import evaluate_conditional
-from .types import Conditional, number, Rule
+from .types import Conditional, Number, Rule
 from .validators import constant_schema, CustomValidationError, variable_schema, rule_schema, validate_schema_with_custom_errors
 from jsonschema.exceptions import ValidationError
 from typing import Literal, Union
 import jsonschema
 
 
 def assert_valid_rules(rules: list[Rule]):
@@ -14,47 +14,39 @@
 	inconsistencies found
 	"""
 	validate_schema_with_custom_errors(rules, rule_schema)
 
 
 def process_rules(
 	rules: list[Rule],
-	constants: dict[str, Union[number, str]] = {},
-	variables: dict[str, Union[number, str]] = {},
-) -> dict[str, Union[number, str]]:
+	constants: dict[str, Union[Number, str]] = {},
+	variables: dict[str, Union[Number, str]] = {},
+) -> dict[str, Union[Number, str]]:
 	"""
 	Process the rules and execute the result of the actions over the passed variables argument
 
 	This function does not mutate the original variables object passed to it
 	"""
 	try:
 		assert_valid_rules(rules)
 	except CustomValidationError as validation_error:
-		raise Exception(
-			f"Invalid input for 'rules': {str(validation_error)}"
-		) from validation_error
+		raise Exception(f"Invalid input for 'rules': {str(validation_error)}") from validation_error
 	except ValidationError as validation_error:
-		raise Exception(
-			f"Invalid input for 'rules': {str(validation_error)}"
-		) from validation_error
+		raise Exception(f"Invalid input for 'rules': {str(validation_error)}") from validation_error
 
 	try:
 		jsonschema.validate(constants, constant_schema)
 	except ValidationError as validation_error:
-		raise Exception(
-			f"Invalid input for 'constants': {validation_error.message}"
-		) from validation_error
+		raise Exception(f"Invalid input for 'constants': {validation_error.message}") from validation_error
 
 	try:
 		jsonschema.validate(variables, variable_schema)
 	except ValidationError as validation_error:
-		raise Exception(
-			f"Invalid input for 'variables': {validation_error.message}"
-		) from validation_error
-	
+		raise Exception(f"Invalid input for 'variables': {validation_error.message}") from validation_error
+
 	result = variables.copy()
 	for rule in rules:
 		actions = rule["actions"]
 		conditions: Conditional = rule["conditions"]
 
 		# Make sure the condition has one single conditional defined
 		assert_single_conditional(conditions)
```

### Comparing `pragmatic_business_rules-0.4.1/src/pragmatic_business_rules/types.py` & `pragmatic_business_rules-0.5.0/src/pragmatic_business_rules/types.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,22 +1,30 @@
 from __future__ import annotations
 from decimal import Decimal
 from typing import Literal, Optional, TypedDict, Union
 
-number = Union[Decimal, int, float]
+Number = Union[Decimal, int, float]
+Operator = Literal[
+	"equal_to",
+	"greater_than_or_equal_to",
+	"greater_than",
+	"less_than_or_equal_to",
+	"less_than",
+	"in",
+]
+
 
 class Action(TypedDict):
-	set: Optional[Union[number, str]]
+	set: Optional[Union[Number, str]]
 
 
 class Condition(TypedDict):
 	constant: Optional[str]
-	operator: Literal["equal_to", "greater_than_or_equal_to", "greater_than",
-										"less_than_or_equal_to", "less_than"]
-	value: Optional[Union[number, str]]
+	operator: Operator
+	value: Optional[Union[Number, list[Number], str, list[str]]]
 	variable: Optional[str]
 
 
 class Conditional(TypedDict):
 	all: Optional[list[Union[Conditional, Condition]]]
 	any: Optional[list[Union[Conditional, Condition]]]
```

### Comparing `pragmatic_business_rules-0.4.1/src/pragmatic_business_rules/validators.py` & `pragmatic_business_rules-0.5.0/src/pragmatic_business_rules/validators.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from jsonschema.exceptions import ValidationError
 from typing import Any
 import jsonschema
 
-class CustomValidationError(Exception):
 
+class CustomValidationError(Exception):
 	def __init__(self, message: str):
 		self.message = message
 		super().__init__(self.message)
 
 
 def validate_schema_with_custom_errors(data: Any, schema: dict):
 	try:
@@ -15,21 +15,23 @@
 	except ValidationError as e:
 		error_message = e.schema.get("error_message")
 		if error_message is not None:
 			raise CustomValidationError(f"{error_message}: {e.message}")
 		else:
 			raise e
 
+
 # This object will match any object with no nested properties and all items being
 # either None, strings or numbers
 constant_schema = {
 	"additionalProperties": False,
 	"patternProperties": {
 		".+": {
 			"type": [
+				"array",
 				"null",
 				"number",
 				"string",
 			]
 		},
 	},
 	"type": "object",
@@ -38,119 +40,141 @@
 # This object will match any object with no nested properties and all items being
 # either None, strings or numbers
 variable_schema = {
 	"additionalProperties": False,
 	"patternProperties": {
 		".+": {
 			"type": [
+				"array",
 				"null",
 				"number",
 				"string",
 			]
 		},
 	},
 	"type": "object",
 }
 
 rule_schema = {
-	"$defs": {
-		"condition": {
-			"additionalProperties": False,
-			"properties": {
-				"constant": {
-					"type": "string",
-				},
-				"operator": {
-					"enum": [
-						"equal_to",
-						"greater_than_or_equal_to",
-						"greater_than",
-						"less_than_or_equal_to",
-						"less_than",
-					],
-					"error_message": "The provided operator for the condition is invalid",
-					"type": "string",
-				},
-				"value": {
-					"type": [
-						"null",
-						"number",
-						"string",
-					],
-				},
-				"variable": {
-					"type": "string",
-				},
-			},
-			"required": [
-				"operator",
-			],
-			"type": "object",
-		},
-		"conditional": {
-			"additionalProperties": False,
-			"properties": {
-				"all": {
-					"items": {
-						"oneOf": [
-							{
-								"$ref": "#/$defs/condition",
-							},
-							{
-								"$ref": "#/$defs/conditional",
-							},
-						],
-					},
-					"type": "array",
-				},
-				"any": {
-					"items": {
-						"oneOf": [
-							{
-								"$ref": "#/$defs/condition",
+	"$defs":
+		{
+			"condition":
+				{
+					"additionalProperties": False,
+					"properties":
+						{
+							"constant": {
+								"type": "string",
 							},
-							{
-								"$ref": "#/$defs/conditional",
-							},
-						],
-					},
-					"type": "array",
-				},
-			},
-			"type": "object"
-		},
-	},
-	"items": {
-		"additionalProperties": False,
-		"properties": {
-			"actions": {
-				"additionalProperties": False,
-				"patternProperties": {
-					".+": {
-						"additionalProperties": False,
-						"patternProperties": {
-							".+": {
-								"error_message": "The provided type for the action is invalid",
+							"operator":
+								{
+									"enum":
+										[
+											"equal_to",
+											"greater_than_or_equal_to",
+											"greater_than",
+											"in",
+											"less_than_or_equal_to",
+											"less_than",
+										],
+									"error_message": "The provided operator for the condition is invalid",
+									"type": "string",
+								},
+							"value": {
 								"type": [
+									"array",
 									"null",
 									"number",
 									"string",
 								],
 							},
+							"variable": {
+								"type": "string",
+							},
+						},
+					"required": ["operator", ],
+					"type": "object",
+				},
+			"conditional":
+				{
+					"additionalProperties": False,
+					"properties":
+						{
+							"all":
+								{
+									"items":
+										{
+											"oneOf":
+												[
+													{
+														"$ref": "#/$defs/condition",
+													},
+													{
+														"$ref": "#/$defs/conditional",
+													},
+												],
+										},
+									"type": "array",
+								},
+							"any":
+								{
+									"items":
+										{
+											"oneOf":
+												[
+													{
+														"$ref": "#/$defs/condition",
+													},
+													{
+														"$ref": "#/$defs/conditional",
+													},
+												],
+										},
+									"type": "array",
+								},
 						},
-						"type": "object",
+					"type": "object"
+				},
+		},
+	"items":
+		{
+			"additionalProperties": False,
+			"properties":
+				{
+					"actions":
+						{
+							"additionalProperties": False,
+							"patternProperties":
+								{
+									".+":
+										{
+											"additionalProperties": False,
+											"patternProperties":
+												{
+													".+":
+														{
+															"error_message":
+																"The provided type for the action is invalid",
+															"type": [
+																"null",
+																"number",
+																"string",
+															],
+														},
+												},
+											"type": "object",
+										},
+								},
+							"type": "object",
+						},
+					"conditions": {
+						"$ref": "#/$defs/conditional",
 					},
 				},
-				"type": "object",
-			},
-			"conditions": {
-				"$ref": "#/$defs/conditional",
-			},
+			"required": [
+				"actions",
+				"conditions",
+			],
+			"type": "object",
 		},
-		"required": [
-			"actions",
-			"conditions",
-		],
-		"type": "object",
-	},
 	"type": "array",
 }
```

### Comparing `pragmatic_business_rules-0.4.1/tests/test_action.py` & `pragmatic_business_rules-0.5.0/tests/test_action.py`

 * *Files identical despite different names*

### Comparing `pragmatic_business_rules-0.4.1/tests/test_condition.py` & `pragmatic_business_rules-0.5.0/tests/test_condition.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,486 +1,522 @@
 from decimal import Decimal
 from src.pragmatic_business_rules.condition import assert_single_conditional, evaluate_condition, evaluate_conditional
 import pytest
 
 
 class TestAssertSingleConditional:
-
 	def test_single_conditional(self):
-		with pytest.raises(
-			Exception,
-			match="'all' and 'any' properties can't be specified for the same conditional"
-		):
+		with pytest.raises(Exception, match="'all' and 'any' properties can't be specified for the same conditional"):
 			assert_single_conditional({"all": [], "any": []})
 
 	def test_valid_conditional(self):
-		with pytest.raises(
-			Exception,
-			match="'all' or 'any' properties were not found in the conditional"
-		):
+		with pytest.raises(Exception, match="'all' or 'any' properties were not found in the conditional"):
 			assert_single_conditional({})
 
 
-class TestEvaluateCondition:
+class TestOperator:
+	def test_in(self):
+		constant_name = "asd"
+		assert evaluate_condition(
+			{
+			"constant": constant_name,
+			"operator": "in",
+			"value": [1, 2]
+			},
+			{constant_name: 1},
+			{},
+		)
+
+		assert not evaluate_condition(
+			{
+			"constant": constant_name,
+			"operator": "in",
+			"value": [2]
+			},
+			{constant_name: 1},
+			{},
+		)
 
+
+class TestEvaluateCondition:
 	def test_constant_exists(self):
 		constant = "xyz"
 		with pytest.raises(Exception, match=f"Constant '{constant}' not defined"):
 			evaluate_condition(
 				{
-					"constant": constant,
-					"operator": "equal_to",
-					"value": "something"
+				"constant": constant,
+				"operator": "equal_to",
+				"value": "something"
 				},
 				{},
 				{},
 			)
 
 	def test_variable_exists(self):
 		variable = "xyz"
 		with pytest.raises(Exception, match=f"Variable '{variable}' not defined"):
 			evaluate_condition(
 				{
-					"variable": variable,
-					"operator": "equal_to",
-					"value": "something"
+				"variable": variable,
+				"operator": "equal_to",
+				"value": "something"
 				},
 				{},
 				{},
 			)
 
 	def test_constant_matches_type(self):
 		constant_name = "abc"
 		constant_value = 1
 		condition_value = "a string"
 		with pytest.raises(
 			Exception,
 			match='\\("{}", "{}", {}\\) and \\("{}", {}\\)'.format(
-				constant_name,
-				constant_value,
-				type(constant_value).__name__,
-				condition_value,
-				type(condition_value).__name__,
+			constant_name,
+			constant_value,
+			type(constant_value).__name__,
+			condition_value,
+			type(condition_value).__name__,
 			),
 		):
 			evaluate_condition(
 				{
-					"constant": constant_name,
-					"operator": "equal_to",
-					"value": condition_value,
+				"constant": constant_name,
+				"operator": "equal_to",
+				"value": condition_value,
 				},
 				{
-					constant_name: constant_value,
+				constant_name: constant_value,
 				},
 				{},
 			)
 
 	def test_variable_matches_type(self):
 		variable_name = "abc"
 		variable_value = 1
 		condition_value = "a string"
 		with pytest.raises(
 			Exception,
 			match='\\("{}", "{}", {}\\) and \\("{}", {}\\)'.format(
-				variable_name,
-				variable_value,
-				type(variable_value).__name__,
-				condition_value,
-				type(condition_value).__name__,
+			variable_name,
+			variable_value,
+			type(variable_value).__name__,
+			condition_value,
+			type(condition_value).__name__,
 			),
 		):
 			evaluate_condition(
 				{
-					"variable": variable_name,
-					"operator": "equal_to",
-					"value": condition_value,
+				"variable": variable_name,
+				"operator": "equal_to",
+				"value": condition_value,
 				},
 				{},
 				{
-					variable_name: variable_value,
+				variable_name: variable_value,
 				},
 			)
 
 	def test_compares_between_number_types(self):
 		constant_name = "abc"
 		constant_value = 1
 		condition_value = 1.5
 		assert not evaluate_condition(
 			{
-				"constant": constant_name,
-				"operator": "equal_to",
-				"value": condition_value,
+			"constant": constant_name,
+			"operator": "equal_to",
+			"value": condition_value,
 			},
 			{
-				constant_name: constant_value,
+			constant_name: constant_value,
 			},
 			{},
 		)
 
 		variable_name = "abc"
 		variable_value = 1.5
 		condition_value = 1
 		assert not evaluate_condition(
 			{
-				"variable": variable_name,
-				"operator": "equal_to",
-				"value": condition_value,
+			"variable": variable_name,
+			"operator": "equal_to",
+			"value": condition_value,
 			},
 			{},
 			{
-				variable_name: variable_value,
+			variable_name: variable_value,
 			},
 		)
 
 		variable_name = "abc"
 		variable_value = 5
 		condition_value = 5.0
 		assert evaluate_condition(
 			{
-				"variable": variable_name,
-				"operator": "equal_to",
-				"value": condition_value,
+			"variable": variable_name,
+			"operator": "equal_to",
+			"value": condition_value,
 			},
 			{},
 			{
-				variable_name: variable_value,
+			variable_name: variable_value,
 			},
 		)
 
 		constant_name = "some"
 		constant_value = Decimal(5)
 		condition_value = 5
 		assert evaluate_condition(
 			{
-				"constant": constant_name,
-				"operator": "equal_to",
-				"value": condition_value,
+			"constant": constant_name,
+			"operator": "equal_to",
+			"value": condition_value,
 			},
 			{
-				constant_name: constant_value,
+			constant_name: constant_value,
 			},
 			{},
 		)
 
+	def test_fails_on_invalid_list_operations(self):
+		constant_name = "somea"
+		operator = "equal_to"
+		with pytest.raises(Exception, match="Can\'t compare between two list values"):
+			evaluate_condition(
+				{
+				"constant": constant_name,
+				"operator": "equal_to",
+				"value": [2],
+				},
+				{
+				constant_name: [1],
+				},
+				{},
+			)
+
+		constant_name = "somea"
+		operator = "equal_to"
+		with pytest.raises(Exception, match="The operator '{}' is not valid for list operations".format(operator, )):
+			evaluate_condition(
+				{
+				"constant": constant_name,
+				"operator": "equal_to",
+				"value": 123,
+				},
+				{
+				constant_name: [1],
+				},
+				{},
+			)
+
 	def test_invalid_type(self):
 		variable = "123"
 		value = {}
 		with pytest.raises(
 			Exception,
-			match="The value '{}' has a type '{}' which is not valid for a condition value"
-			.format(
-				value,
-				type(value).__name__,
+			match="The value '{}' has a type '{}' which is not valid for a condition value".format(
+			value,
+			type(value).__name__,
 			)
 		):
 			evaluate_condition(
 				{
-					"variable": variable,
-					"operator": "equal_to",
-					"value": value,
+				"variable": variable,
+				"operator": "equal_to",
+				"value": value,
 				},
 				{},
 				{
-					variable: {},
+				variable: {},
 				},
 			)
 
 	def test_string_comparable_to_none(self):
 		variable = "variable name"
 
 		assert not evaluate_condition(
 			{
-				"variable": variable,
-				"operator": "equal_to",
-				"value": None,
+			"variable": variable,
+			"operator": "equal_to",
+			"value": None,
 			},
 			{},
 			{
-				variable: "some value",
+			variable: "some value",
 			},
 		)
 
 	def test_none_comparable_to_none(self):
 		variable = "not a variable name"
 
 		assert evaluate_condition(
 			{
-				"variable": variable,
-				"operator": "equal_to",
-				"value": None,
+			"variable": variable,
+			"operator": "equal_to",
+			"value": None,
 			},
 			{},
 			{
-				variable: None,
+			variable: None,
 			},
 		)
 
 	def test_string_equal_to(self):
 		variable = "some variable"
 		value = "some value"
 
 		assert evaluate_condition(
 			{
-				"variable": variable,
-				"operator": "equal_to",
-				"value": value,
+			"variable": variable,
+			"operator": "equal_to",
+			"value": value,
 			},
 			{},
 			{
-				variable: value,
+			variable: value,
 			},
 		)
 
 		assert not evaluate_condition(
 			{
-				"variable": variable,
-				"operator": "equal_to",
-				"value": value,
+			"variable": variable,
+			"operator": "equal_to",
+			"value": value,
 			},
 			{},
 			{
-				variable: value + " other",
+			variable: value + " other",
 			},
 		)
 
 	def test_invalid_string_operator(self):
 		variable = "123"
 		operator = "invalid operator"
-		with pytest.raises(
-			Exception,
-			match=f"The operator '{operator}' is not valid for string operations"
-		):
+		with pytest.raises(Exception, match=f"The operator '{operator}' is not valid for string operations"):
 			evaluate_condition(
 				{
-					"variable": variable,
-					"operator": operator,
-					"value": "123",
+				"variable": variable,
+				"operator": operator,
+				"value": "123",
 				},
 				{},
 				{
-					variable: "asd",
+				variable: "asd",
 				},
 			)
 
 	def test_number_equal_to(self):
 		variable = "some variable"
 		value = 15
 
 		assert evaluate_condition(
 			{
-				"variable": variable,
-				"operator": "equal_to",
-				"value": value,
+			"variable": variable,
+			"operator": "equal_to",
+			"value": value,
 			},
 			{},
 			{
-				variable: value,
+			variable: value,
 			},
 		)
 
 		assert not evaluate_condition(
 			{
-				"variable": variable,
-				"operator": "equal_to",
-				"value": value,
+			"variable": variable,
+			"operator": "equal_to",
+			"value": value,
 			},
 			{},
 			{
-				variable: value + 10,
+			variable: value + 10,
 			},
 		)
 
 	def test_number_greater_than_or_equal_to(self):
 		variable = "some variable"
 		value = 450.54
 
 		assert evaluate_condition(
 			{
-				"variable": variable,
-				"operator": "greater_than_or_equal_to",
-				"value": value,
+			"variable": variable,
+			"operator": "greater_than_or_equal_to",
+			"value": value,
 			},
 			{},
 			{
-				variable: value,
+			variable: value,
 			},
 		)
 
 		assert evaluate_condition(
 			{
-				"variable": variable,
-				"operator": "greater_than_or_equal_to",
-				"value": value - 1,
+			"variable": variable,
+			"operator": "greater_than_or_equal_to",
+			"value": value - 1,
 			},
 			{},
 			{
-				variable: value,
+			variable: value,
 			},
 		)
 
 		assert not evaluate_condition(
 			{
-				"variable": variable,
-				"operator": "greater_than_or_equal_to",
-				"value": value + 1,
+			"variable": variable,
+			"operator": "greater_than_or_equal_to",
+			"value": value + 1,
 			},
 			{},
 			{
-				variable: value,
+			variable: value,
 			},
 		)
 
 	def test_number_greater_than(self):
 		variable = "some variable"
 		value = 125
 
 		assert evaluate_condition(
 			{
-				"variable": variable,
-				"operator": "greater_than",
-				"value": value - 1,
+			"variable": variable,
+			"operator": "greater_than",
+			"value": value - 1,
 			},
 			{},
 			{
-				variable: value,
+			variable: value,
 			},
 		)
 
 		assert not evaluate_condition(
 			{
-				"variable": variable,
-				"operator": "greater_than",
-				"value": value,
+			"variable": variable,
+			"operator": "greater_than",
+			"value": value,
 			},
 			{},
 			{
-				variable: value,
+			variable: value,
 			},
 		)
 
 		assert not evaluate_condition(
 			{
-				"variable": variable,
-				"operator": "greater_than",
-				"value": value + 1,
+			"variable": variable,
+			"operator": "greater_than",
+			"value": value + 1,
 			},
 			{},
 			{
-				variable: value,
+			variable: value,
 			},
 		)
 
 	def test_number_less_than_or_equal_to(self):
 		variable = "some variable"
 		value = 521350.879821
 
 		assert evaluate_condition(
 			{
-				"variable": variable,
-				"operator": "less_than_or_equal_to",
-				"value": value + 1,
+			"variable": variable,
+			"operator": "less_than_or_equal_to",
+			"value": value + 1,
 			},
 			{},
 			{
-				variable: value,
+			variable: value,
 			},
 		)
 
 		assert evaluate_condition(
 			{
-				"variable": variable,
-				"operator": "less_than_or_equal_to",
-				"value": value,
+			"variable": variable,
+			"operator": "less_than_or_equal_to",
+			"value": value,
 			},
 			{},
 			{
-				variable: value,
+			variable: value,
 			},
 		)
 
 		assert not evaluate_condition(
 			{
-				"variable": variable,
-				"operator": "less_than_or_equal_to",
-				"value": value - 1,
+			"variable": variable,
+			"operator": "less_than_or_equal_to",
+			"value": value - 1,
 			},
 			{},
 			{
-				variable: value,
+			variable: value,
 			},
 		)
 
 	def test_number_less_than(self):
 		variable = "some variable"
 		value = 48.5316541
 
 		assert evaluate_condition(
 			{
-				"variable": variable,
-				"operator": "less_than",
-				"value": value + 1,
+			"variable": variable,
+			"operator": "less_than",
+			"value": value + 1,
 			},
 			{},
 			{
-				variable: value,
+			variable: value,
 			},
 		)
 
 		assert not evaluate_condition(
 			{
-				"variable": variable,
-				"operator": "less_than",
-				"value": value,
+			"variable": variable,
+			"operator": "less_than",
+			"value": value,
 			},
 			{},
 			{
-				variable: value,
+			variable: value,
 			},
 		)
 
 		assert not evaluate_condition(
 			{
-				"variable": variable,
-				"operator": "less_than",
-				"value": value - 1,
+			"variable": variable,
+			"operator": "less_than",
+			"value": value - 1,
 			},
 			{},
 			{
-				variable: value,
+			variable: value,
 			},
 		)
 
 	def test_invalid_number_operator(self):
 		variable = "number variable"
 		operator = "invalid operator"
-		with pytest.raises(
-			Exception,
-			match=f"The operator '{operator}' is not valid for number operations"
-		):
+		with pytest.raises(Exception, match=f"The operator '{operator}' is not valid for number operations"):
 			evaluate_condition(
 				{
-					"variable": variable,
-					"operator": operator,
-					"value": 0,
+				"variable": variable,
+				"operator": operator,
+				"value": 0,
 				},
 				{},
 				{
-					variable: 1,
+				variable: 1,
 				},
 			)
 
 
 class TestEvaluateConditional:
-
 	def test_invalid_type(self):
 		type = "something else"
-		with pytest.raises(
-			Exception,
-			match=f"The evaluation type '{type}' is not a valid conditional type"
-		):
+		with pytest.raises(Exception, match=f"The evaluation type '{type}' is not a valid conditional type"):
 			evaluate_conditional(
 				[],
 				{},
 				{},
 				type,
 			)
 
@@ -492,605 +528,621 @@
 		variable_1 = "some variable"
 		value_1 = 123
 		variable_2 = "some other variable"
 		value_2 = "xyz"
 
 		assert evaluate_conditional(
 			[
-				{
-					"variable": variable_1,
-					"operator": "equal_to",
-					"value": value_1,
-				},
-				{
-					"variable": variable_2,
-					"operator": "equal_to",
-					"value": value_2,
-				},
+			{
+			"variable": variable_1,
+			"operator": "equal_to",
+			"value": value_1,
+			},
+			{
+			"variable": variable_2,
+			"operator": "equal_to",
+			"value": value_2,
+			},
 			],
 			{},
 			{
-				variable_1: value_1,
-				variable_2: value_2,
+			variable_1: value_1,
+			variable_2: value_2,
 			},
 			"all",
 		)
 
 		assert evaluate_conditional(
 			[
-				{
-					"variable": variable_1,
-					"operator": "equal_to",
-					"value": value_1,
-				},
+			{
+			"variable": variable_1,
+			"operator": "equal_to",
+			"value": value_1,
+			},
 			],
 			{},
 			{
-				variable_1: value_1,
+			variable_1: value_1,
 			},
 			"all",
 		)
 
 		assert not evaluate_conditional(
 			[
-				{
-					"variable": variable_1,
-					"operator": "equal_to",
-					"value": value_1,
-				},
-				{
-					"variable": variable_2,
-					"operator": "equal_to",
-					"value": value_2 + "123",
-				},
+			{
+			"variable": variable_1,
+			"operator": "equal_to",
+			"value": value_1,
+			},
+			{
+			"variable": variable_2,
+			"operator": "equal_to",
+			"value": value_2 + "123",
+			},
 			],
 			{},
 			{
-				variable_1: value_1,
-				variable_2: value_2,
+			variable_1: value_1,
+			variable_2: value_2,
 			},
 			"all",
 		)
 
 		assert not evaluate_conditional(
 			[
-				{
-					"variable": variable_1,
-					"operator": "equal_to",
-					"value": value_1 + 15,
-				},
+			{
+			"variable": variable_1,
+			"operator": "equal_to",
+			"value": value_1 + 15,
+			},
 			],
 			{},
 			{
-				variable_1: value_1,
+			variable_1: value_1,
 			},
 			"all",
 		)
 
 	def test_all_conditions_nested(self):
 		variable_1 = "some variable"
 		value_1 = 6487
 		variable_2 = "some other variable"
 		value_2 = "asdjn"
 		variable_3 = "some other other variable"
 		value_3 = 4580.1
 
 		assert evaluate_conditional(
 			[
-				{
-					"all": [
-						{
-							"variable": variable_1,
-							"operator": "equal_to",
-							"value": value_1,
-						},
-						{
-							"variable": variable_2,
-							"operator": "equal_to",
-							"value": value_2,
-						},
-					],
-				},
-				{
-					"all": [{
-						"variable": variable_3,
-						"operator": "equal_to",
-						"value": value_3,
-					}],
-				},
+			{
+			"all":
+			[
+			{
+			"variable": variable_1,
+			"operator": "equal_to",
+			"value": value_1,
+			},
+			{
+			"variable": variable_2,
+			"operator": "equal_to",
+			"value": value_2,
+			},
+			],
+			},
+			{
+			"all": [{
+			"variable": variable_3,
+			"operator": "equal_to",
+			"value": value_3,
+			}],
+			},
 			],
 			{},
 			{
-				variable_1: value_1,
-				variable_2: value_2,
-				variable_3: value_3,
+			variable_1: value_1,
+			variable_2: value_2,
+			variable_3: value_3,
 			},
 			"all",
 		)
 
 		assert evaluate_conditional(
 			[
-				{
-					"all": [
-						{
-							"variable": variable_1,
-							"operator": "equal_to",
-							"value": value_1,
-						},
-						{
-							"variable": variable_2,
-							"operator": "equal_to",
-							"value": value_2,
-						},
-					],
-				},
+			{
+			"all":
+			[
+			{
+			"variable": variable_1,
+			"operator": "equal_to",
+			"value": value_1,
+			},
+			{
+			"variable": variable_2,
+			"operator": "equal_to",
+			"value": value_2,
+			},
+			],
+			},
 			],
 			{},
 			{
-				variable_1: value_1,
-				variable_2: value_2,
+			variable_1: value_1,
+			variable_2: value_2,
 			},
 			"all",
 		)
 
 		assert not evaluate_conditional(
 			[
-				{
-					"all": [
-						{
-							"variable": variable_1,
-							"operator": "equal_to",
-							"value": value_1,
-						},
-						{
-							"variable": variable_2,
-							"operator": "equal_to",
-							"value": value_2 + "something",
-						},
-					],
-				},
-				{
-					"all": [{
-						"variable": variable_3,
-						"operator": "equal_to",
-						"value": value_3,
-					}],
-				},
+			{
+			"all":
+			[
+			{
+			"variable": variable_1,
+			"operator": "equal_to",
+			"value": value_1,
+			},
+			{
+			"variable": variable_2,
+			"operator": "equal_to",
+			"value": value_2 + "something",
+			},
+			],
+			},
+			{
+			"all": [{
+			"variable": variable_3,
+			"operator": "equal_to",
+			"value": value_3,
+			}],
+			},
 			],
 			{},
 			{
-				variable_1: value_1,
-				variable_2: value_2,
-				variable_3: value_3,
+			variable_1: value_1,
+			variable_2: value_2,
+			variable_3: value_3,
 			},
 			"all",
 		)
 
 		assert not evaluate_conditional(
 			[
-				{
-					"all": [
-						{
-							"variable": variable_1,
-							"operator": "equal_to",
-							"value": value_1,
-						},
-						{
-							"variable": variable_2,
-							"operator": "equal_to",
-							"value": value_2 + "something",
-						},
-					],
-				},
-				{
-					"all": [{
-						"variable": variable_3,
-						"operator": "equal_to",
-						"value": value_3 + 17,
-					}],
-				},
+			{
+			"all":
+			[
+			{
+			"variable": variable_1,
+			"operator": "equal_to",
+			"value": value_1,
+			},
+			{
+			"variable": variable_2,
+			"operator": "equal_to",
+			"value": value_2 + "something",
+			},
+			],
+			},
+			{
+			"all": [{
+			"variable": variable_3,
+			"operator": "equal_to",
+			"value": value_3 + 17,
+			}],
+			},
 			],
 			{},
 			{
-				variable_1: value_1,
-				variable_2: value_2,
-				variable_3: value_3,
+			variable_1: value_1,
+			variable_2: value_2,
+			variable_3: value_3,
 			},
 			"all",
 		)
 
 	def test_any_conditions(self):
 		variable_1 = "some variable"
 		value_1 = 47.5
 		variable_2 = "some other variable"
 		value_2 = "A1"
 
 		assert evaluate_conditional(
 			[
-				{
-					"variable": variable_1,
-					"operator": "equal_to",
-					"value": value_1,
-				},
-				{
-					"variable": variable_2,
-					"operator": "equal_to",
-					"value": value_2,
-				},
+			{
+			"variable": variable_1,
+			"operator": "equal_to",
+			"value": value_1,
+			},
+			{
+			"variable": variable_2,
+			"operator": "equal_to",
+			"value": value_2,
+			},
 			],
 			{},
 			{
-				variable_1: value_1,
-				variable_2: value_2,
+			variable_1: value_1,
+			variable_2: value_2,
 			},
 			"any",
 		)
 
 		assert evaluate_conditional(
 			[
-				{
-					"variable": variable_1,
-					"operator": "equal_to",
-					"value": value_1,
-				},
-				{
-					"variable": variable_2,
-					"operator": "equal_to",
-					"value": value_2 + "asd",
-				},
+			{
+			"variable": variable_1,
+			"operator": "equal_to",
+			"value": value_1,
+			},
+			{
+			"variable": variable_2,
+			"operator": "equal_to",
+			"value": value_2 + "asd",
+			},
 			],
 			{},
 			{
-				variable_1: value_1,
-				variable_2: value_2,
+			variable_1: value_1,
+			variable_2: value_2,
 			},
 			"any",
 		)
 
 		assert not evaluate_conditional(
 			[
-				{
-					"variable": variable_1,
-					"operator": "equal_to",
-					"value": value_1 + 10,
-				},
-				{
-					"variable": variable_2,
-					"operator": "equal_to",
-					"value": value_2 + "123",
-				},
+			{
+			"variable": variable_1,
+			"operator": "equal_to",
+			"value": value_1 + 10,
+			},
+			{
+			"variable": variable_2,
+			"operator": "equal_to",
+			"value": value_2 + "123",
+			},
 			],
 			{},
 			{
-				variable_1: value_1,
-				variable_2: value_2,
+			variable_1: value_1,
+			variable_2: value_2,
 			},
 			"any",
 		)
 
 	def test_any_conditions_nested(self):
 		variable_1 = "some variable"
 		value_1 = 19
 		variable_2 = "some other variable"
 		value_2 = "keeping"
 		variable_3 = "some other other variable"
 		value_3 = 5123.45
 
 		assert evaluate_conditional(
 			[
-				{
-					"any": [
-						{
-							"variable": variable_1,
-							"operator": "equal_to",
-							"value": value_1,
-						},
-						{
-							"variable": variable_2,
-							"operator": "equal_to",
-							"value": value_2,
-						},
-					],
-				},
-				{
-					"any": [{
-						"variable": variable_3,
-						"operator": "equal_to",
-						"value": value_3,
-					},],
-				},
+			{
+			"any":
+			[
+			{
+			"variable": variable_1,
+			"operator": "equal_to",
+			"value": value_1,
+			},
+			{
+			"variable": variable_2,
+			"operator": "equal_to",
+			"value": value_2,
+			},
+			],
+			},
+			{
+			"any": [{
+			"variable": variable_3,
+			"operator": "equal_to",
+			"value": value_3,
+			}, ],
+			},
 			],
 			{},
 			{
-				variable_1: value_1,
-				variable_2: value_2,
-				variable_3: value_3,
+			variable_1: value_1,
+			variable_2: value_2,
+			variable_3: value_3,
 			},
 			"any",
 		)
 
 		assert evaluate_conditional(
 			[
-				{
-					"any": [
-						{
-							"variable": variable_1,
-							"operator": "equal_to",
-							"value": value_1,
-						},
-						{
-							"variable": variable_2,
-							"operator": "equal_to",
-							"value": value_2 + "something",
-						},
-					],
-				},
-				{
-					"any": [{
-						"variable": variable_3,
-						"operator": "equal_to",
-						"value": value_3,
-					}],
-				},
+			{
+			"any":
+			[
+			{
+			"variable": variable_1,
+			"operator": "equal_to",
+			"value": value_1,
+			},
+			{
+			"variable": variable_2,
+			"operator": "equal_to",
+			"value": value_2 + "something",
+			},
+			],
+			},
+			{
+			"any": [{
+			"variable": variable_3,
+			"operator": "equal_to",
+			"value": value_3,
+			}],
+			},
 			],
 			{},
 			{
-				variable_1: value_1,
-				variable_2: value_2,
-				variable_3: value_3,
+			variable_1: value_1,
+			variable_2: value_2,
+			variable_3: value_3,
 			},
 			"any",
 		)
 
 		assert evaluate_conditional(
 			[
-				{
-					"any": [
-						{
-							"variable": variable_1,
-							"operator": "equal_to",
-							"value": value_1,
-						},
-						{
-							"variable": variable_2,
-							"operator": "equal_to",
-							"value": value_2 + "something",
-						},
-					],
-				},
-				{
-					"any": [{
-						"variable": variable_3,
-						"operator": "equal_to",
-						"value": value_3 + 15156416,
-					}],
-				},
+			{
+			"any":
+			[
+			{
+			"variable": variable_1,
+			"operator": "equal_to",
+			"value": value_1,
+			},
+			{
+			"variable": variable_2,
+			"operator": "equal_to",
+			"value": value_2 + "something",
+			},
+			],
+			},
+			{
+			"any": [{
+			"variable": variable_3,
+			"operator": "equal_to",
+			"value": value_3 + 15156416,
+			}],
+			},
 			],
 			{},
 			{
-				variable_1: value_1,
-				variable_2: value_2,
-				variable_3: value_3,
+			variable_1: value_1,
+			variable_2: value_2,
+			variable_3: value_3,
 			},
 			"any",
 		)
 
 		assert not evaluate_conditional(
 			[
-				{
-					"any": [
-						{
-							"variable": variable_1,
-							"operator": "equal_to",
-							"value": value_1 + 54164,
-						},
-						{
-							"variable": variable_2,
-							"operator": "equal_to",
-							"value": value_2 + "something",
-						},
-					],
-				},
-				{
-					"any": [{
-						"variable": variable_3,
-						"operator": "equal_to",
-						"value": value_3 + 17,
-					}],
-				},
+			{
+			"any":
+			[
+			{
+			"variable": variable_1,
+			"operator": "equal_to",
+			"value": value_1 + 54164,
+			},
+			{
+			"variable": variable_2,
+			"operator": "equal_to",
+			"value": value_2 + "something",
+			},
+			],
+			},
+			{
+			"any": [{
+			"variable": variable_3,
+			"operator": "equal_to",
+			"value": value_3 + 17,
+			}],
+			},
 			],
 			{},
 			{
-				variable_1: value_1,
-				variable_2: value_2,
-				variable_3: value_3,
+			variable_1: value_1,
+			variable_2: value_2,
+			variable_3: value_3,
 			},
 			"any",
 		)
 
 	def test_mixed_conditions_nested(self):
 		variable_1 = "some variable"
 		value_1 = 41684
 		variable_2 = "some other variable"
 		value_2 = "clancy"
 		variable_3 = "some other other variable"
 		value_3 = 178.45
 
 		assert evaluate_conditional(
 			[
-				{
-					"any": [
-						{
-							"variable": variable_1,
-							"operator": "equal_to",
-							"value": value_1,
-						},
-						{
-							"variable": variable_2,
-							"operator": "equal_to",
-							"value": value_2 + "asd",
-						},
-					],
-				},
-				{
-					"all": [{
-						"variable": variable_3,
-						"operator": "equal_to",
-						"value": value_3,
-					}],
-				},
+			{
+			"any":
+			[
+			{
+			"variable": variable_1,
+			"operator": "equal_to",
+			"value": value_1,
+			},
+			{
+			"variable": variable_2,
+			"operator": "equal_to",
+			"value": value_2 + "asd",
+			},
+			],
+			},
+			{
+			"all": [{
+			"variable": variable_3,
+			"operator": "equal_to",
+			"value": value_3,
+			}],
+			},
 			],
 			{},
 			{
-				variable_1: value_1,
-				variable_2: value_2,
-				variable_3: value_3,
+			variable_1: value_1,
+			variable_2: value_2,
+			variable_3: value_3,
 			},
 			"any",
 		)
 
 		assert not evaluate_conditional(
 			[
-				{
-					"all": [
-						{
-							"variable": variable_1,
-							"operator": "equal_to",
-							"value": value_1,
-						},
-						{
-							"variable": variable_2,
-							"operator": "equal_to",
-							"value": value_2 + "something",
-						},
-					],
-				},
+			{
+			"all":
+			[
+			{
+			"variable": variable_1,
+			"operator": "equal_to",
+			"value": value_1,
+			},
+			{
+			"variable": variable_2,
+			"operator": "equal_to",
+			"value": value_2 + "something",
+			},
+			],
+			},
 			],
 			{},
 			{
-				variable_1: value_1,
-				variable_2: value_2,
-				variable_3: value_3,
+			variable_1: value_1,
+			variable_2: value_2,
+			variable_3: value_3,
 			},
 			"any",
 		)
 
 		assert evaluate_conditional(
 			[
-				{
-					"all": [
-						{
-							"variable": variable_1,
-							"operator": "equal_to",
-							"value": value_1,
-						},
-						{
-							"any": [
-								{
-									"variable": variable_2,
-									"operator": "equal_to",
-									"value": value_2 + "something",
-								},
-								{
-									"variable": variable_3,
-									"operator": "equal_to",
-									"value": value_3,
-								},
-							]
-						},
-					],
-				},
+			{
+			"all":
+			[
+			{
+			"variable": variable_1,
+			"operator": "equal_to",
+			"value": value_1,
+			},
+			{
+			"any":
+			[
+			{
+			"variable": variable_2,
+			"operator": "equal_to",
+			"value": value_2 + "something",
+			},
+			{
+			"variable": variable_3,
+			"operator": "equal_to",
+			"value": value_3,
+			},
+			]
+			},
+			],
+			},
 			],
 			{},
 			{
-				variable_1: value_1,
-				variable_2: value_2,
-				variable_3: value_3,
+			variable_1: value_1,
+			variable_2: value_2,
+			variable_3: value_3,
 			},
 			"all",
 		)
 
 		assert not evaluate_conditional(
 			[
-				{
-					"all": [
-						{
-							"variable": variable_1,
-							"operator": "equal_to",
-							"value": value_1,
-						},
-						{
-							"any": [
-								{
-									"variable": variable_2,
-									"operator": "equal_to",
-									"value": value_2 + "something",
-								},
-								{
-									"all": [
-										{
-											"variable": variable_1,
-											"operator": "equal_to",
-											"value": value_1,
-										},
-										{
-											"variable": variable_3,
-											"operator": "equal_to",
-											"value": value_3 + 245152,
-										},
-									]
-								},
-							]
-						},
-					],
-				},
+			{
+			"all":
+			[
+			{
+			"variable": variable_1,
+			"operator": "equal_to",
+			"value": value_1,
+			},
+			{
+			"any":
+			[
+			{
+			"variable": variable_2,
+			"operator": "equal_to",
+			"value": value_2 + "something",
+			},
+			{
+			"all":
+			[
+			{
+			"variable": variable_1,
+			"operator": "equal_to",
+			"value": value_1,
+			},
+			{
+			"variable": variable_3,
+			"operator": "equal_to",
+			"value": value_3 + 245152,
+			},
+			]
+			},
+			]
+			},
+			],
+			},
 			],
 			{},
 			{
-				variable_1: value_1,
-				variable_2: value_2,
-				variable_3: value_3,
+			variable_1: value_1,
+			variable_2: value_2,
+			variable_3: value_3,
 			},
 			"any",
 		)
 
+
 class TestConditionalInputs:
 	def test_invalid_categories(self):
 		with pytest.raises(
 			Exception,
 			match='No values were found',
 		):
 			evaluate_condition(
 				{
-					"operator": "equal_to",
+				"operator": "equal_to",
 				},
 				{},
 				{},
 			)
 
 		with pytest.raises(
 			Exception,
 			match='"value" found',
 		):
 			evaluate_condition(
 				{
-					"value": "some value",
-					"operator": "equal_to",
+				"value": "some value",
+				"operator": "equal_to",
 				},
 				{},
 				{},
 			)
 
 		with pytest.raises(
 			Exception,
 			match='"constant, value, variable" found',
 		):
 			evaluate_condition(
 				{
-					"value": "some value",
-					"variable": "some variable",
-					"constant": "some constant",
-					"operator": "equal_to",
+				"value": "some value",
+				"variable": "some variable",
+				"constant": "some constant",
+				"operator": "equal_to",
 				},
 				{},
 				{},
-			)
+			)
```

### Comparing `pragmatic_business_rules-0.4.1/tests/test_main.py` & `pragmatic_business_rules-0.5.0/tests/test_main.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,120 +1,160 @@
 from src.pragmatic_business_rules import process_rules
 import pytest
 
 
-class TestProcessRules:
+class TestGeneral:
+	def test_correct_result(self):
+		var = "result"
+		constant_1 = "c1"
+		constant_1_value = "1"
+		constant_2 = "c2"
+		constant_2_value = 2
+		constant_3 = "c3"
+		constant_3_value_a = "x"
+		constant_3_value_b = ["x", "y"]
+		result = process_rules(
+			[
+				{
+					"actions": {
+						var: {
+							"set": 1
+						}
+					},
+					"conditions":
+						{
+							"all":
+								[
+									{
+										"constant": constant_1,
+										"operator": "equal_to",
+										"value": constant_1_value
+									},
+									{
+										"constant": constant_2,
+										"operator": "equal_to",
+										"value": constant_2_value
+									},
+									{
+										"constant": constant_3,
+										"operator": "in",
+										"value": constant_3_value_b
+									},
+								],
+						}
+				}
+			],
+			{
+				constant_1: constant_1_value,
+				constant_2: constant_2_value,
+				constant_3: constant_3_value_a,
+			},
+			{
+				var: 0,
+			},
+		)
+
+		assert result[var] == 1
 
+
+class TestProcessRules:
 	def test_assert_rule_schema(self):
 		with pytest.raises(
 			Exception,
 			match="Invalid input for 'rules': 'actions' is a required property",
 		):
-			process_rules(
-				[
-					{
-						"conditions": {
-							"all": [],
-						},
+			process_rules([
+				{
+					"conditions": {
+						"all": [],
 					},
-				],
-			)
+				},
+			], )
 
 		with pytest.raises(
 			Exception,
 			match="Invalid input for 'rules': The provided type for the action is invalid",
 		):
-			process_rules(
-				[
-					{
-						"actions": {
-							"unknown rule": {
-								"set": True,
-							},
-						},
-						"conditions": {
-							"all": [],
+			process_rules([
+				{
+					"actions": {
+						"unknown rule": {
+							"set": True,
 						},
 					},
-				],
-			)
+					"conditions": {
+						"all": [],
+					},
+				},
+			], )
 
 		with pytest.raises(
 			Exception,
 			match="Invalid input for 'rules': The provided operator for the condition is invalid",
 		):
 			process_rules(
 				[
 					{
 						"actions": {},
-						"conditions": {
-							"all": [{
-								"variable": "variable",
-								"operator": "invalid operator",
-								"value": 1,
-							}],
-						},
+						"conditions":
+							{
+								"all": [{
+									"variable": "variable",
+									"operator": "invalid operator",
+									"value": 1,
+								}],
+							},
 					},
 				],
 			)
 
 	def test_assert_constant_schema(self):
 		with pytest.raises(
 			Exception,
-			match="Invalid input for 'constants': {} is not of type 'null', 'number', 'string'",
+			match="Invalid input for 'constants': {} is not of type",
 		):
 			process_rules(
 				[],
 				constants={
 					"an object": {},
 				},
 			)
 
 	def test_assert_variable_schema(self):
 		with pytest.raises(
 			Exception,
-			match="Invalid input for 'variables': {} is not of type 'null', 'number', 'string'",
+			match="Invalid input for 'variables': {} is not of type",
 		):
 			process_rules(
 				[],
 				variables={
 					"an object": {},
 				},
 			)
 
 	def test_assert_single_conditional(self):
-		with pytest.raises(
-			Exception,
-			match="'all' and 'any' properties can't be specified for the same conditional"
-		):
-			process_rules(
-				[
-					{
-						"actions": {},
-						"conditions": {
-							"all": [],
-							"any": []
-						},
+		with pytest.raises(Exception, match="'all' and 'any' properties can't be specified for the same conditional"):
+			process_rules([
+				{
+					"actions": {},
+					"conditions": {
+						"all": [],
+						"any": []
 					},
-				],
-			)
+				},
+			], )
 
 	def test_assert_valid_conditional(self):
-		with pytest.raises(
-			Exception,
-			match="'all' or 'any' properties were not found in the conditional"
-		):
-			process_rules(
-				[
-					{
-						"actions": {},
-						"conditions": {},
-					},
-				],
-			)
+		with pytest.raises(Exception, match="'all' or 'any' properties were not found in the conditional"):
+			process_rules([
+				{
+					"actions": {},
+					"conditions": {},
+				},
+			], )
 
 	def test_apply_no_action(self):
 		item_name = "single key"
 		current_item_value = 42.12
 		expected_item_value = 99
 		variable_name = "some variable"
 		variable_value = "xyz"
@@ -123,21 +163,25 @@
 			[
 				{
 					"actions": {
 						item_name: {
 							"set": expected_item_value
 						}
 					},
-					"conditions": {
-						"any": [{
-							"variable": variable_name,
-							"operator": "equal_to",
-							"value": variable_value + "abc",
-						}],
-					}
+					"conditions":
+						{
+							"any":
+								[
+									{
+										"variable": variable_name,
+										"operator": "equal_to",
+										"value": variable_value + "abc",
+									}
+								],
+						}
 				},
 			],
 			variables={
 				item_name: current_item_value,
 				variable_name: variable_value,
 			},
 		)
@@ -154,21 +198,22 @@
 			[
 				{
 					"actions": {
 						item_name: {
 							"set": item_value
 						}
 					},
-					"conditions": {
-						"any": [{
-							"constant": constant_name,
-							"operator": "equal_to",
-							"value": constant_value,
-						}],
-					}
+					"conditions":
+						{
+							"any": [{
+								"constant": constant_name,
+								"operator": "equal_to",
+								"value": constant_value,
+							}],
+						}
 				},
 			],
 			constants={
 				constant_name: constant_value,
 			},
 			variables={
 				item_name: item_value - 1,
@@ -188,21 +233,22 @@
 			[
 				{
 					"actions": {
 						item_name: {
 							"set": expected_item_value
 						}
 					},
-					"conditions": {
-						"any": [{
-							"variable": variable_name,
-							"operator": "less_than",
-							"value": variable_value,
-						}],
-					}
+					"conditions":
+						{
+							"any": [{
+								"variable": variable_name,
+								"operator": "less_than",
+								"value": variable_value,
+							}],
+						}
 				},
 			],
 			variables={
 				item_name: expected_item_value - 1,
 				variable_name: variable_value,
 			},
 		)
@@ -223,42 +269,45 @@
 			[
 				{
 					"actions": {
 						variable_1_name: {
 							"set": variable_1_value
 						}
 					},
-					"conditions": {
-						"any": [{
-							"constant": constant_1_name,
-							"operator": "equal_to",
-							"value": constant_1_value,
-						}],
-					}
+					"conditions":
+						{
+							"any": [{
+								"constant": constant_1_name,
+								"operator": "equal_to",
+								"value": constant_1_value,
+							}],
+						}
 				},
 				{
 					"actions": {
 						variable_2_name: {
 							"set": variable_2_value
 						}
 					},
-					"conditions": {
-						"all": [
-							{
-								"constant": constant_1_name,
-								"operator": "equal_to",
-								"value": constant_1_value,
-							},
-							{
-								"constant": constant_2_name,
-								"operator": "equal_to",
-								"value": constant_2_value,
-							},
-						],
-					}
+					"conditions":
+						{
+							"all":
+								[
+									{
+										"constant": constant_1_name,
+										"operator": "equal_to",
+										"value": constant_1_value,
+									},
+									{
+										"constant": constant_2_name,
+										"operator": "equal_to",
+										"value": constant_2_value,
+									},
+								],
+						}
 				},
 			],
 			constants={
 				constant_1_name: constant_1_value,
 				constant_2_name: constant_2_value,
 			},
 			variables={
@@ -333,21 +382,25 @@
 				[
 					{
 						"actions": {
 							constant_1_name: {
 								"set": 1
 							}
 						},
-						"conditions": {
-							"any": [{
-								"constant": constant_2_name,
-								"operator": "equal_to",
-								"value": constant_2_value,
-							}],
-						}
+						"conditions":
+							{
+								"any":
+									[
+										{
+											"constant": constant_2_name,
+											"operator": "equal_to",
+											"value": constant_2_value,
+										}
+									],
+							}
 					},
 				],
 				constants={
 					constant_1_name: 0,
 					constant_2_name: constant_2_value
 				}
-			)
+			)
```

### Comparing `pragmatic_business_rules-0.4.1/tests/test_validators.py` & `pragmatic_business_rules-0.5.0/tests/test_validators.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,109 +1,102 @@
 from decimal import Decimal
 from jsonschema.exceptions import ValidationError
 from src.pragmatic_business_rules.validators import rule_schema, variable_schema
 import jsonschema
 import pytest
 
+
 def test_conditions():
 	jsonschema.validate(
 		[
 			{
 				"actions": {},
-				"conditions": {
-					"any": [
-						{
-							"variable": "some variable",
-							"constant": "some constant",
-							"operator": "equal_to",
-							"value": "something"
-						}
-					]
-				}
+				"conditions":
+					{
+						"any":
+							[
+								{
+									"variable": "some variable",
+									"constant": "some constant",
+									"operator": "equal_to",
+									"value": "something"
+								}
+							]
+					}
 			}
 		],
 		rule_schema,
 	)
-	
+
 	with pytest.raises(ValidationError) as variable_error:
 		jsonschema.validate(
-			[
-				{
-					"actions": {},
-					"conditions": {
-						"any": [
-							{
-								"variable": 1,
-							}
-						]
-					}
+			[{
+				"actions": {},
+				"conditions": {
+					"any": [{
+						"variable": 1,
+					}]
 				}
-			],
+			}],
 			rule_schema,
 		)
 
 	assert variable_error.value.json_path == "$[0].conditions.any[0].variable"
 	assert variable_error.value.validator == "type"
 
 	with pytest.raises(ValidationError) as constant_error:
 		jsonschema.validate(
-			[
-				{
-					"actions": {},
-					"conditions": {
-						"any": [
-							{
-								"constant": 1,
-							}
-						]
-					}
+			[{
+				"actions": {},
+				"conditions": {
+					"any": [{
+						"constant": 1,
+					}]
 				}
-			],
+			}],
 			rule_schema,
 		)
 
 	assert constant_error.value.json_path == "$[0].conditions.any[0].constant"
 	assert constant_error.value.validator == "type"
 
 	with pytest.raises(ValidationError) as operator_error:
 		jsonschema.validate(
-			[
-				{
-					"actions": {},
-					"conditions": {
-						"any": [
-							{
-								"variable": "asd",
-							}
-						]
-					}
+			[{
+				"actions": {},
+				"conditions": {
+					"any": [{
+						"variable": "asd",
+					}]
 				}
-			],
+			}],
 			rule_schema,
 		)
 
 	assert operator_error.value.json_path == "$[0].conditions.any[0]"
 	assert operator_error.value.validator == "required"
 
+
 def test_plain_dictionary_schema():
 	jsonschema.validate({}, variable_schema)
 	jsonschema.validate(
 		{
+			"array": [1, 2],
 			"string": "some string",
 			"int": 1,
 			"float": 2.5,
 			"decimal": Decimal(12),
 			"none": None,
 		},
 		variable_schema,
 	)
 
 	with pytest.raises(
 		ValidationError,
-		match="{} is not of type 'null', 'number', 'string'",
+		match="{} is not of type",
 	):
 		jsonschema.validate(
 			{
 				"an object": {},
 			},
 			variable_schema,
 		)
```

### Comparing `pragmatic_business_rules-0.4.1/LICENSE` & `pragmatic_business_rules-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pragmatic_business_rules-0.4.1/pyproject.toml` & `pragmatic_business_rules-0.5.0/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "pragmatic-business-rules"
-version = "0.4.1"
+version = "0.5.0"
 authors = [{ name = "Soremwar", email = "stephenguerrero43@gmail.com" }]
 description = "Pragmatic business rules"
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
 	"License :: OSI Approved :: MIT License",
 	"Operating System :: OS Independent",
@@ -19,7 +19,13 @@
 
 [build-system]
 requires = ["hatchling", "hatch-requirements-txt"]
 build-backend = "hatchling.build"
 
 [tool.hatch.metadata.hooks.requirements_txt]
 files = ["requirements.txt"]
+
+[tool.yapf]
+based_on_style = "facebook"
+column_limit = 120
+continuation_align_style = "valign-right"
+use_tabs = true
```

### Comparing `pragmatic_business_rules-0.4.1/PKG-INFO` & `pragmatic_business_rules-0.5.0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: pragmatic-business-rules
-Version: 0.4.1
+Version: 0.5.0
 Summary: Pragmatic business rules
 Project-URL: Homepage, https://github.com/Soremwar/pragmatic_business_rules
 Project-URL: Issues, https://github.com/Soremwar/pragmatic_business_rules/issues
 Author-email: Soremwar <stephenguerrero43@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

