# Creating a DNS record in VTA to access student samba

- In side panel of your openstack project
- Navigate to DNS >> Zones
- Click "Create Zone"
- The name field can be anything, but it will have to end in "vta." (be sure to include the period at the end)
    - Example: "test.vta."
    - Example: "student.vta."
- The email field can be any fake email (ex. fake@fake.com)
- Click "Submit"
- Click on "Create Record Set"
- Leave "A - Address Record" selected in the "Type" dropdown
- In the "Name" field, enter the name of the subdomain you want to create
    - Example: "jack.test.vta." (be sure to include the period at the end)
    - Example: "vm1.student.vta."
- Under "Record" enter the IP address of the server you want to point to
    - Example: 10.50.X.X
    - Example: 192.168.X.X (Only accessible if instance trying to connect is on the same network)
- Click "Submit"
- Access samba through file browser with documented instructions.
