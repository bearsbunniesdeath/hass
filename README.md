# hass
Home Assistant configurations for my house

# Setup
1. Create secrets.yaml file and add the following secrets:
- hikvision_username: "<USERNAME HERE>"
- hikvision_password: "<PASSWORD HERE>"
2. Update paths in compose.yml
3. Copy contents from super duper secret secrets folder into this directory

# Post-init setup
1. Add cameras using UI
- Still image URL: http://<nvr_ip>/ISAPI/ContentMgmt/StreamingProxy/channels/<camera_number>01/picture
- Stream source URL: rtsp://<nvr_ip>:554/ISAPI/Streaming/channels/<camera_number>01/
- UDP transport
- Digest authentication
- NVR user and password
- Don't verify SSL
2. Add Airthings integration
- Get API key and secret from Airthings website

