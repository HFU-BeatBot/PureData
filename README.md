# Pure Data

Pure Data (PD) is an open source visual programming language for multimedia.
It is used for sound editing and realtime audio processing among other things.
One goal of this project is to find a way to access the EasyMlServe Server in PD and send with PD generated MFCC values to it. This task is splitted in two subtasks: Generating MFCC and send the HTML POST request.

## Pure Data Website

Download and install [Pure Data](https://puredata.info/).

## PuRestJson

Natively PD has no practical way to handle HTTP-requests, but there is an extension which implements this.

[Link to PuRestJson Github](https://github.com/residuum/PuRestJson)

### How to install PuRestJson:

1. Open PD
2. Go to `help`
3. Open `find externals online`
4. Search `purest_json`
5. Install the shown extension

### Use file from the repo

1. Open PD
2. Open the file `server-request.pd` via `file` -> `open`

## MFCC values

There is no native way to determine the MFCC values of a sound file.

### melf~

There was an older version with an object called `melf~` that might have done what we wanted, but it was removed in the newer versions because it was deprecated. Installing an older version made it available, but without any proper documentation or instructions on how to use it.

### VampPlugins

VampPlugins is a library designed to work with sound files from the console. They have proposed to implement the given functionality in PD, but no one has done it in the last 15 years.

[Link to VampPlugins](https://puredata.info/dev/summer-of-code/VampPlugins)

### MC-Sonaar

All in all, this seems relatively interesting, but it's not useful for our context because it only generates 13 out of 20 MFCC values and no mean or default value.
So this won't work for us.

[Link to MC-Sonaar](https://github.com/GiantSteps/MC-Sonaar)

## Conclusion

Generating the JSON Request is doable. The generating of the MFCC values is to complex for the last weeks of this semester project.
