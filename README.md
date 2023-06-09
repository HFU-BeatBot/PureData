# Pure Data

Pure Data (PD) is an open source visual programming language for multimedia.
It is used for sound editing and realtime audio processing among other things.
One goal of this project is to find a way to access the EasyMlServe Server in PD.

### Pure Data Website
https://puredata.info/

Download and install Pure Data.

### PuRestJson
Natively PD has no practical way to handle HTTP-requests, but there is an extension which implements this.
https://github.com/residuum/PuRestJson

How to install PuRestJson:
1. Open PD
2. Go to `help`
3. Open `find externals online`
4. Search `purest_json`
5. Install the shown extension

### Use file from the repo

1. Open PD
2. Open the file `server-request.pd` via `file` -> `open`