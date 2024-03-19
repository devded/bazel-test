o install Bazel on Linux, you can follow these steps:

Update Package Lists: First, ensure your package lists are up to date by running:

sql
Copy code
sudo apt update
Install Required Dependencies: Bazel has some dependencies that need to be installed beforehand. You can install them using:

Copy code
sudo apt install curl gnupg
Add Bazel's package distribution URI and key: Run the following commands to add Bazel's package distribution URI and key to your system:

bash
Copy code
echo "deb [arch=amd64] https://storage.googleapis.com/bazel-apt stable jdk1.8" | sudo tee /etc/apt/sources.list.d/bazel.list
curl https://bazel.build/bazel-release.pub.gpg | sudo apt-key add -
Update Package Lists (again): Update your package lists to include the new Bazel repository:

sql
Copy code
sudo apt update
Install Bazel: Finally, install Bazel using the following command:

Copy code
sudo apt install bazel
Verify Installation: Once the installation is complete, you can verify it by checking the version of Bazel:

css
Copy code
bazel --version




sudo apt update
sudo apt install curl gnupg
echo "deb [arch=amd64] https://storage.googleapis.com/bazel-apt stable jdk1.8" | sudo tee /etc/apt/sources.list.d/bazel.list
curl https://bazel.build/bazel-release.pub.gpg | sudo apt-key add -
sudo apt update
sudo apt install bazel
bazel --version