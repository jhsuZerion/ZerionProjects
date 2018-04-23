# RippleNami - Uganda Taxpayer Project
## Technologies Used
- iFormBuilder White Label (rCAPTURE)
- Dataflow Automation
   - Actions
      - iFormBuilder Record
      - HTTP REQUEST (GET)
      - HTTP REQUEST (PUT)
## Testing Environment Setup
- Import the Form Package [Package_RippleNami Uganda 4_22.json](https://github.com/jhsuZerion/ZerionProjects/blob/master/ripplenami/uganda/Package_RippleNami%20Uganda%204_22.json)
- Import the Dataflow [Uganda Dataflow.json](https://github.com/jhsuZerion/ZerionProjects/blob/master/ripplenami/uganda/Uganda%20Dataflow.json)
- Update the Dataflow Action `add_property_unique_id` 
   - Create and/or assign a valid iFormBuilder Connection
   - Select form named `registration_c_property`
   - Map `property_unique_id` to `record['property_unique_id']`
- Create iFormBuilder Endpoint with Webhook URL from `ifb_registration_p`
- Double-check that the Action `PUT_rwaves_prod` is disabled
## Test Cases
*For each test case, if a new property is registered, check in iFormBuilder for the property_unique_id which is the parish_id + record ID.  
If a new property is registered, check the Residential Properties layer in [rWAVES Staging](https://rwaves-stage.ripplenami.com/web/index.html#/maps/mine/).  
If a new or existing individual is included in the record, check the corresponding layer in [rWAVES Staging](https://rwaves-stage.ripplenami.com/web/index.html#/maps/mine/) based on the `registration_relationship` field.*
- [ ] Complete rCAPTURE record filling in new property with no individual
- [ ] How to Test: Complete rCAPTURE record filling in new property with new individual
- [ ] How to Test: Complete rCAPTURE record filling in new property with existing individual
- [ ] Complete rCAPTURE record selecting existing property with new individual
- [ ] Complete rCAPTURE record selecting existing property with existing individual
## Test History
