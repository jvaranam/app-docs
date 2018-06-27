#Installing gradle in mac / ios

Here is the solution I found for Mac

Download the Gradle Binary Only Distribution from https://gradle.org/gradle-download/

Open a terminal
Run the following to unzip the android sdk to the Development directory that is under your user home directory

unzip ~/Downloads/gradle-3.1-bin.zip -d ~/Development
Open up the vi editor and edit your bash profile. We need to add in the GRADLE_HOME environment variable

vi ~/.bash_profile
To edit in vi hit i to enter edit mode and add the text below to the .bash_profile

export GRADLE_HOME=~/Development/gradle-3.1/bin
Press the esc key to exit edit mode
Press : (colon key) to enter command mode.
type wq and press enter to save and exit vi
Run the following to make the change active in your existing session

source ~/.bash_profile
Test it by running

echo $GRADLE_HOME
