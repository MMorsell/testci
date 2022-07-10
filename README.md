# Create a folder
$ mkdir actions-runner && cd actions-runner# Download the latest runner package
$ curl -o actions-runner-linux-x64-2.294.0.tar.gz -L https://github.com/actions/runner/releases/download/v2.294.0/actions-runner-linux-x64-2.294.0.tar.gz# Optional: Validate the hash
$ echo "a19a09f4eda5716e5d48ba86b6b78fc014880c5619b9dba4a059eaf65e131780  actions-runner-linux-x64-2.294.0.tar.gz" | shasum -a 256 -c# Extract the installer
$ tar xzf ./actions-runner-linux-x64-2.294.0.tar.gz
Configure
# Create the runner and start the configuration experience
$ ./config.sh --url https://github.com/MMorsell/testci --token AMFIA3CLRPZRNGE2IVBZMOLCZMLYK# Last step, run it!
$ ./run.sh
