# RippleNami - Uganda Taxpayer Project
## Technologies Used
- iFormBuilder White Label (rCAPTURE)
- Dataflow Automation
   - Actions
      - iFormBuilder Record
      - HTTP REQUEST (GET)
      - HTTP REQUEST (PUT)
## Test Cases
- [ ] Register New Property without Individual
   - How to Test: Complete rCAPTURE record filling in new property with no individual
   - Success Criteria:
      - iFormBuilder record updated with property index
      - New rWAVES pin on Residential Properties layer
- [ ] Register New Property with New Individual
   - How to Test: Complete rCAPTURE record filling in new property with new individual
   - Success Criteria:
      - iFormBuilder record updated with property index
      - New rWAVES pin on Residential Properties layer
      - New rWAVES pin on Individual layer depending on relationship selected in record
- [ ] Register New Property with Existing Individual
   - How to Test: Complete rCAPTURE record filling in new property with existing individual
   - Success Criteria:
      - iFormBuilder record updated with property index
      - New rWAVES pin on Residential Properties layer
      - New rWAVES pin on Individual layer depending on relationship selected in record
- [ ] Register Existing Property with New Individual
   - How to Test: Complete rCAPTURE record selecting existing property with new individual
   - Success Criteria: 
      - New rWAVES pin on Residential Properties layer
      - New rWAVES pin on Individual layer depending on relationship selected in record
- [ ] Register Existing Property with Existing Individual
   - How to Test: Complete rCAPTURE record selecting existing property with existing individual
   - Success Criteria: 
      - New rWAVES pin on Residential Properties layer
      - New rWAVES pin on Individual layer depending on relationship selected in record
## Test History
