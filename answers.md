"POST /devices" with the probe body
- Status: 201
- Number of devices: 5

"POST /devices" with the probe body, again
- Status: 201
- Number of devices: 6
- Notes: The probe device was duplicated



"PUT /devices/attic" with the attic body
- Status: 200
- Number of devices: 6

"PUT /devices/attic" with the attic body, again
- Status: 200
- Number of devices: 6
- Notes: attic body was replaced with itself and did not change



"DELETE /devices/fridge" 
- Status: 200
- Number of devices: 5

"DELETE /devices/fridge", again
- Status: 404
- Number of devices: 5
- Notes: fridge did not exist in the dictinary and returns an error

