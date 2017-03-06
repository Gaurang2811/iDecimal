
#
## Rest API Details for iDecimal

13 th  December 2016

#### Product 1(a) - FIGPlus

###### URL :

[http://111.93.34.137:8080/kie-server/services/rest/server/containers/instances/FIGplus](http://111.93.34.137:8080/kie-server/services/rest/server/containers/instances/FIGplus)

###### Method:

POST

###### Header :

Accept: application/json
Content-Type: application/json

###### Request Payload Description :

| &quot;dhfl\_idecimal.decimal\_dhfl.domain.FIGInput&quot;: {  &quot;policyTerm&quot;: { type : int },  &quot;premiumPaymentTerm&quot;: { type : int},  &quot;premiumPaymentMode&quot;: { type : String         Values : &quot;Annual&quot;, &quot;Semi-Annual&quot;, &quot;Monthly&quot;},  &quot;Age&quot;: { type : int},  &quot;basicSumAssured&quot;: { type : double},  &quot;extraMortalityRate\_rate&quot;: { type : double},  &quot;occupationalFlatExtra\_rate&quot;:{ type : double},  &quot;otherFlatExtra\_rate&quot;:{ type : double},  &quot;nsapFlatExtra\_rate&quot;:{ type : double},  &quot;extraMortalityRate\_optedFor&quot;: { type : String,          Values : &quot;No&quot;, &quot;Yes&quot;},  &quot;occupationalFlatExtra\_optedFor&quot;:{ type : String,          Values : &quot;No&quot;, &quot;Yes&quot;},  &quot;otherFlatExtra\_optedFor&quot;:{ type : String,          Values : &quot;No&quot;, &quot;Yes&quot;},  &quot;nsapFlatExtra\_optedFor&quot;:{ type : String,          Values : &quot;No&quot;, &quot;Yes&quot;}, &quot;extraMortalityRate\_duration&quot;:{ type : Integer}, &quot;occupationalFlatExtra\_duration&quot;:{ type : Integer}, &quot;otherFlatExtra\_duration&quot;:{ type : Integer}, &quot;nsapFlatExtra\_duration&quot;:{ type : Integer},  &quot;dateOfQuotation&quot;: { type : Date},  &quot;nameOfLifeAssured&quot;: { type : String},  &quot;dateOfBirth&quot;: { type : String},  &quot;Sex&quot;: { type : String,    Values : &quot;Male&quot;, &quot;Female&quot;} }  |
| --- |

###### Request Payload Example :

| { &quot;commands&quot;: [   {     &quot;set-global&quot;: {       &quot;identifier&quot;: &quot;outputList&quot;,       &quot;object&quot;: [],       &quot;out-identifier&quot;: &quot;resultList&quot;     }   },   {     &quot;insert&quot;: {       &quot;out-identifier&quot;: &quot;Input&quot;,       &quot;return-object&quot;: &quot;false&quot;,       &quot;object&quot;: {_ _         &quot;dhfl\_idecimal.decimal\_dhfl.domain.FIGInput&quot;: {            &quot;policyTerm&quot;: 25,            &quot;premiumPaymentTerm&quot;: 25,            &quot;premiumPaymentMode&quot;: &quot;Annual&quot;,            &quot;age&quot;: 35,            &quot;basicSumAssured&quot;: 1000000,             &quot;extraMortalityRate\_rate&quot; : 500,             &quot;extraMortalityRate\_duration&quot; : 25,             &quot;extraMortalityRate\_optedFor&quot; : &quot;Yes&quot;,             &quot;occupationalFlatExtra\_rate&quot; : 2,             &quot;occupationalFlatExtra\_duration&quot; : 15,             &quot;occupationalFlatExtra\_optedFor&quot; : &quot;No&quot;,             &quot;otherFlatExtra\_rate&quot; : 5,             &quot;otherFlatExtra\_duration&quot; : 4,             &quot;otherFlatExtra\_optedFor&quot; : &quot;No&quot;,             &quot;nsapFlatExtra\_rate&quot; : 3,             &quot;nsapFlatExtra\_duration&quot; : 10,             &quot;nsapFlatExtra\_optedFor&quot; : &quot;No&quot;,            &quot;dateOfQuotation&quot;:null,            &quot;nameOfLifeAssured&quot;:&quot;Abhishek&quot;,            &quot;dateOfBirth&quot;:null,            &quot;sex&quot;:&quot;Male&quot;         }       }     }   },   {     &quot;fire-all-rules&quot;: {       &quot;outIdentifier&quot;: &quot;output&quot;     }   } ]} |
| --- |

#### Product 1(b) - FIGPlus-Reverse

###### NOTE :  URL, Method Type and ###### Header will be the same as for FIgPlus

###### Request Payload Description :

| &quot;dhfl\_idecimal.decimal\_dhfl.domain.ReverseInput&quot;: {                   &quot;age&quot;: {type : int},                    &quot;sex&quot; : { type : String,          Values : &quot;Male&quot;, &quot;Female&quot;}                   &quot;policyTerm&quot;: {type : int},                   &quot;premiumPaymentTerm&quot;: {type : int},                   &quot;premium&quot;: {type : double},                   &quot;premiumPaymentMode&quot;:  { type : String           Values : &quot;Annual&quot;, &quot;Semi-Annual&quot;, &quot;Monthly&quot;},                   &quot;occupationalFlatExtra\_optedFor&quot;: { type : String,                    Values : &quot;No&quot;, &quot;Yes&quot;},                   &quot;occupationalFlatExtra\_rate&quot;:{ type : double},                   &quot;occupationalFlatExtra\_duration&quot;:{ type : Integer},               }  |
| --- |

###### Request Payload Example :

| {   &quot;commands&quot;: [{       &quot;insert&quot;: {           &quot;out-identifier&quot;: &quot;Input&quot;,           &quot;object&quot;: {                &quot;dhfl\_idecimal.decimal\_dhfl.domain.ReverseInput&quot;: {                    &quot;age&quot;: 35,                     &quot;sex&quot; : &quot;Male&quot;,                    &quot;policyTerm&quot;: 20,                    &quot;premiumPaymentTerm&quot;: 20,                    &quot;premium&quot;: 2000,                    &quot;premiumPaymentMode&quot;: &quot;Monthly&quot;,                               &quot;occupationalFlatExtra\_rate&quot; : 2,                    &quot;occupationalFlatExtra\_duration&quot; : 15,                   &quot;occupationalFlatExtra\_optedFor&quot; : &quot;No&quot;,               }           }       }   },{       &quot;fire-all-rules&quot;: {           &quot;outIdentifier&quot;: null       }   }]}  |
| --- |

#### Product 2 - SmartFeeProtect

###### URL :

[http://111.93.34.137:8080/kie-server/services/rest/server/containers/instances/smartfeeprotect](http://111.93.34.137:8080/kie-server/services/rest/server/containers/instances/smartfeeprotect)

###### Method :

POST

###### Header :

Accept: application/json
Content-Type: application/json

###### Request Payload Description :

| &quot;dhfl\_idecimal.decimal\_dhfl.domain.Input&quot;: {             &quot;isPremium&quot;: {type : BooleanValue : True(for Premium as input), False(for Monthly Income as Input)},              &quot;dateOfQuotation&quot;: { type : Date},              &quot;nameOfLifeAssured&quot;: { type : String},              &quot;dateOfBirth&quot;: { type : String},              &quot;sex&quot;:  { type : String,          Values : &quot;Male&quot;, &quot;Female&quot;},,              &quot;age&quot;: {type : int},              &quot;premiumPaymentMode&quot;: { type : String           Values : &quot;Annual&quot;, &quot;Semi-Annual&quot;, &quot;Monthly&quot;},              &quot;policyTerm&quot;: {type : int},              &quot;premiumPaymentTerm&quot;: {type : int},              &quot;modalPremium&quot;: {type : double(when IsPremium : Ture)},              &quot;monthlyIncome&quot;: {type : double(when IsPremium : False)},              &quot;basePolicyExtraMortalityRate\_optedFor&quot;: { type : String,               Values : &quot;No&quot;, &quot;Yes&quot;},              &quot;basePolicyOccupationalFlatExtra\_optedFor&quot;: { type : String,                     Values : &quot;No&quot;, &quot;Yes&quot;},              &quot;basePolicyOtherFlatExtra\_optedFor&quot;:{ type : String,         Values : &quot;No&quot;, &quot;Yes&quot;},              &quot;basePolicyNsapFlatExtra\_optedFor&quot;:{ type : String,       Values : &quot;No&quot;, &quot;Yes&quot;},                          &quot;basePolicyExtraMortalityRate\_rate&quot;: { type : double},              &quot;basePolicyOccupationalFlatExtra\_rate&quot;: { type : double},              &quot;basePolicyOtherFlatExtra\_rate&quot;: { type : double},              &quot;basePolicyNsapFlatExtra\_rate&quot;: { type : double},              &quot;basePolicyExtraMortalityRate\_duration&quot;:{ type : double},              &quot;basePolicyOccupationalFlatExtra\_duration&quot;:{ type : double},              &quot;basePolicyOtherFlatExtra\_duration&quot;:{ type : double},              &quot;basePolicyNsapFlatExtra\_duration&quot;:{ type : double},              &quot;adbRider&quot;: { type : String,              Values : &quot;No&quot;, &quot;Yes&quot;},              &quot;adbSumAssured&quot;:{ type : double},              &quot;termOfAdbRider&quot;:{ type : int},              &quot;ciRider&quot;: { type : String,           Values : &quot;No&quot;, &quot;Yes&quot;},              &quot;ciSumAssured&quot;:{ type : double},              &quot;termOfCiRider&quot;:{ type : int},              &quot;adbRiderExtraMortalityRate\_optedFor&quot;: { type : String,                  Values : &quot;No&quot;, &quot;Yes&quot;},              &quot;adbRiderFlatExtra\_optedFor&quot;: { type : String,              Values : &quot;No&quot;, &quot;Yes&quot;},              &quot;adbRiderExtraMortalityRate\_rate&quot;: { type : double},              &quot;adbRiderFlatExtra\_rate&quot;:{ type : double},              &quot;adbRiderExtraMortalityRate\_duration&quot;:{ type : double},              &quot;adbRiderFlatExtra\_duration&quot;:{ type : double},              &quot;ciRiderExtraMortalityRate\_optedFor&quot;:{type : String,                        Values : &quot;No&quot;, &quot;Yes&quot;},              &quot;ciRiderFlatExtra\_optedFor&quot;: {type : String,                           Values : &quot;No&quot;, &quot;Yes&quot;},              &quot;ciRiderExtraMortalityRate\_rate&quot;: { type : double},              &quot;ciRiderFlatExtra\_duration&quot;:{ type : double},              &quot;ciRiderExtraMortalityRate\_rate&quot;: { type : double},              &quot;ciRiderFlatExtra\_duration&quot;:{ type : double}, } |
| --- |

###### Request Payload Example :

| {  &quot;commands&quot;: [    {      &quot;set-global&quot;: {        &quot;identifier&quot;: &quot;output&quot;,        &quot;object&quot;: [],        &quot;out-identifier&quot;: &quot;resultList&quot;      }    },    {      &quot;insert&quot;: {        &quot;out-identifier&quot;: &quot;Input&quot;,        &quot;return-object&quot;: &quot;false&quot;,        &quot;object&quot;: {           &quot;dhfl\_idecimal.decimal\_dhfl.domain.Input&quot;: {               &quot;isPremium&quot;:true,               &quot;dateOfQuotation&quot;:null,               &quot;nameOfLifeAssured&quot;:&quot;XYZ&quot;,               &quot;dateOfBirth&quot;:null,               &quot;sex&quot;:&quot;Female&quot;,               &quot;Age&quot;:50,                 &quot;premiumPaymentMode&quot;:&quot;Annual&quot;,               &quot;policyTerm&quot;:10,               &quot;premiumPaymentTerm&quot;:7,               &quot;modalPremium&quot;:50000,               &quot;monthlyIncome&quot;:10000,                 &quot;basePolicyExtraMortalityRate\_optedFor&quot;:&quot;No&quot;,               &quot;basePolicyOccupationalFlatExtra\_optedFor&quot;:&quot;Yes&quot;,               &quot;basePolicyOtherFlatExtra\_optedFor&quot;:&quot;No&quot;,               &quot;basePolicyNsapFlatExtra\_optedFor&quot;:&quot;No&quot;,                            &quot;basePolicyExtraMortalityRate\_rate&quot;:0.5,               &quot;basePolicyOccupationalFlatExtra\_rate&quot;:2,               &quot;basePolicyOtherFlatExtra\_rate&quot;:7,               &quot;basePolicyNsapFlatExtra\_rate&quot;:2,                            &quot;basePolicyExtraMortalityRate\_duration&quot;:7,               &quot;basePolicyOccupationalFlatExtra\_duration&quot;:7,               &quot;basePolicyOtherFlatExtra\_duration&quot;:7,               &quot;basePolicyNsapFlatExtra\_duration&quot;:7,                 &quot;adbRider&quot;:&quot;No&quot;,               &quot;adbSumAssured&quot;:300000,               &quot;termOfAdbRider&quot;:5,               &quot;ciRider&quot;:&quot;No&quot;,               &quot;ciSumAssured&quot;:105000,               &quot;termOfCiRider&quot;:6,                 &quot;adbRiderExtraMortalityRate\_optedFor&quot;:&quot;No&quot;,               &quot;adbRiderFlatExtra\_optedFor&quot;:&quot;No&quot;,               &quot;adbRiderExtraMortalityRate\_rate&quot;:1.25,               &quot;adbRiderFlatExtra\_rate&quot;:8,               &quot;adbRiderExtraMortalityRate\_duration&quot;:5,               &quot;adbRiderFlatExtra\_duration&quot;:5,                 &quot;ciRiderExtraMortalityRate\_optedFor&quot;:&quot;No&quot;,               &quot;ciRiderFlatExtra\_optedFor&quot;:&quot;No&quot;,               &quot;ciRiderExtraMortalityRate\_rate&quot;:0.71,               &quot;ciRiderFlatExtra\_rate&quot;:5,               &quot;ciRiderExtraMortalityRate\_duration&quot;:0.13,               &quot;ciRiderFlatExtra\_duration&quot;:5           }      }    }    },    {      &quot;fire-all-rules&quot;: {        &quot;outIdentifier&quot;: &quot;output&quot;      }    }  ]} |
| --- |

#### Product 3(a) - FlexiCash

###### URL :

[http://111.93.34.137:8080/kie-server/services/rest/server/containers/instances/flexicash](http://111.93.34.137:8080/kie-server/services/rest/server/containers/instances/flexicash)

###### Method :

POST

###### Header :

Accept: application/json
Content-Type: application/json

###### Request Payload Description :

| &quot;dhfl\_idecimal.decimal\_dhfl.domain.FlexiCashInput&quot;: {  &quot;policyTerm&quot;: { type : int },  &quot;premiumPaymentMode&quot;: { type : String         Values : &quot;Annual&quot;, &quot;Semi-Annual&quot;, &quot;Monthly&quot;},  &quot;Age&quot;: { type : int},  &quot;basicSumAssured&quot;: { type : double}, &quot;extraMortalityRate\_rate&quot;: { type : double},  &quot;occupationalFlatExtra\_rate&quot;:{ type : double},  &quot;otherFlatExtra\_rate&quot;:{ type : double},  &quot;nsapFlatExtra\_rate&quot;:{ type : double},  &quot;extraMortalityRate\_optedFor&quot;: { type : String,          Values : &quot;No&quot;, &quot;Yes&quot;},  &quot;occupationalFlatExtra\_optedFor&quot;:{ type : String,          Values : &quot;No&quot;, &quot;Yes&quot;},  &quot;otherFlatExtra\_optedFor&quot;:{ type : String,          Values : &quot;No&quot;, &quot;Yes&quot;},  &quot;nsapFlatExtra\_optedFor&quot;:{ type : String,          Values : &quot;No&quot;, &quot;Yes&quot;}, &quot;extraMortalityRate\_duration&quot;:{ type : Integer}, &quot;occupationalFlatExtra\_duration&quot;:{ type : Integer}, &quot;otherFlatExtra\_duration&quot;:{ type : Integer}, &quot;nsapFlatExtra\_duration&quot;:{ type : Integer},  &quot;dateOfQuotation&quot;: { type : Date},  &quot;nameOfLifeAssured&quot;: { type : String},  &quot;dateOfBirth&quot;: { type : Date},  &quot;Sex&quot;: { type : String,    Values : &quot;Male&quot;, &quot;Female&quot;} } |
| --- |

###### Request Payload Example :

| { &quot;commands&quot;: [   {     &quot;set-global&quot;: {       &quot;identifier&quot;: &quot;outputList&quot;,       &quot;object&quot;: [],       &quot;out-identifier&quot;: &quot;resultList&quot;     }   },   {     &quot;insert&quot;: {       &quot;out-identifier&quot;: &quot;Input&quot;,       &quot;return-object&quot;: &quot;false&quot;,       &quot;object&quot;: {          &quot;dhfl\_idecimal.decimal\_dhfl.domain.FlexiCashInput&quot;: {            &quot;policyTerm&quot;: 35,            &quot;premiumPaymentMode&quot;: &quot;Annual&quot;,            &quot;age&quot;: 35,            &quot;basicSumAssured&quot;: 1000000,              &quot;extraMortalityRate\_rate&quot; : 500,             &quot;extraMortalityRate\_duration&quot; : 25,             &quot;extraMortalityRate\_optedFor&quot; : &quot;Yes&quot;,             &quot;occupationalFlatExtra\_rate&quot; : 2,             &quot;occupationalFlatExtra\_duration&quot; : 15,             &quot;occupationalFlatExtra\_optedFor&quot; : &quot;No&quot;,             &quot;otherFlatExtra\_rate&quot; : 5,             &quot;otherFlatExtra\_duration&quot; : 4,             &quot;otherFlatExtra\_optedFor&quot; : &quot;No&quot;,             &quot;nsapFlatExtra\_rate&quot; : 3,             &quot;nsapFlatExtra\_duration&quot; : 10,             &quot;nsapFlatExtra\_optedFor&quot; : &quot;No&quot;,            &quot;dateOfQuotation&quot;:null,            &quot;nameOfLifeAssured&quot;:&quot;Abhishek&quot;,            &quot;dateOfBirth&quot;:null,            &quot;sex&quot;:&quot;Male&quot;         }       }     }   },   {     &quot;fire-all-rules&quot;: {       &quot;outIdentifier&quot;: &quot;output&quot;     }   } ]} |
| --- |

#### Product 3(b) - FlexiCash-Reverse

###### NOTE : URL, Method Type and ###### Header will be the same as for FlexiCash

###### Request Payload Description :

| &quot;dhfl\_idecimal.decimal\_dhfl.domain.ReverseInput&quot;: {                   &quot;age&quot;: {type : int},                    &quot;sex&quot; : { type : String,          Values : &quot;Male&quot;, &quot;Female&quot;}                   &quot;policyTerm&quot;: {type : int},                   &quot;premium&quot;: {type : double},                   &quot;premiumPaymentMode&quot;:  { type : String           Values : &quot;Annual&quot;, &quot;Semi-Annual&quot;, &quot;Monthly&quot;},                   &quot;occupationalFlatExtra\_optedFor&quot;: { type : String,                    Values : &quot;No&quot;, &quot;Yes&quot;},                   &quot;occupationalFlatExtra\_rate&quot;:{ type : double},                   &quot;occupationalFlatExtra\_duration&quot;:{ type : Integer}               }  |
| --- |

###### Request Payload Example :

| {   &quot;commands&quot;: [{       &quot;insert&quot;: {           &quot;out-identifier&quot;: &quot;Input&quot;,           &quot;object&quot;: {                &quot;dhfl\_idecimal.decimal\_dhfl.domain.ReverseInput&quot;: {                    &quot;age&quot;: 35,                     &quot;sex&quot; : &quot;Male&quot;,                    &quot;policyTerm&quot;: 35,                    &quot;premium&quot;: 500000,                    &quot;premiumPaymentMode&quot;: &quot;Monthly&quot;,                    &quot;occupationalFlatExtra\_rate&quot; : 2,                    &quot;occupationalFlatExtra\_duration&quot; : 15,                   &quot;occupationalFlatExtra\_optedFor&quot; : &quot;No&quot;,                }           }       }   },{       &quot;fire-all-rules&quot;: {           &quot;outIdentifier&quot;: null       }   }]} |
| --- |

