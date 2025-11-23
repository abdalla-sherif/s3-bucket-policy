# AccessoryPacket S3 Project

*Description:* Access restricted S3 object accessible only via my IP.

## Project Overview
This project demonstrates how to control access to a specific S3 object within an S3 bucket named AccessoryPacket. The goal was to make the object accessible only from a specific IP address.

## Steps Taken
1. Created an S3 bucket named AccessoryPacket using AWS CLI.
2. Uploaded an object to the bucket via AWS CLI.
3. Disabled the bucket's *Block Public Access* settings.
4. Enabled read access for everyone at the object level temporarily to confirm the object was accessible.
5. Created a *Bucket Policy* in JSON format restricting access to only my IP address.
6. Applied the policy using AWS CLI.
7. Verified that the object can now be accessed only from the specified IP.

## Notes
- The object is not public; only requests from the configured IP can access it.
- All actions were performed using AWS CLI.
