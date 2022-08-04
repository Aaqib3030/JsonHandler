# JsonHandler
This is an Apex class for Salesforce. This class takes any multi level JSON String as an input and returns a single level Json containing all the paths of the leaf nodes as keys and leaf node values as the values.

For Example - 

if the input Json is like the one below.
{
  "Username": "Bob",
  "Address": {
    "Street": "19th main",
    "House no": 80,
    "Locality": "HBR",
    "pincode": 560034
  },
  "phone": 83095
}

Then the output will be like - 
{
  "/Username": "Bob",
  "/Address/pincode": 560034,
  "/Address/Locality": "HBR",
  "/Address/House no": 80,
  "/Address/Street": "19th main",
  "/phone": 83095
}

NOTE : The Logic implemented can be used in any language
