# SSH Setup

## Step 1: Check for Existing SSH Keys

Open Powershell as an Administrator.

Navigate to the directory C.

Run `ls ~/.ssh`

If you see files like id_rsa and id_rsa.pub, you already have an SSH key. You can skip key generation and proceed to Step 3.

If no such files exist, proceed to Step 2 to generate a new SSH key.

## Step 2: Generate a New SSH Key

Generate the key via the following command ensuring you are using the email associated with your GitHub account: `ssh-keygen -t ed25519 -C "your_email@example.com"`

Verify that the key was created via the following command: `ls ~/.ssh`
You should see id_ed25519 (private key) and id_ed25519.pub (public key).

## Step 3: Check whether SSH-Agent is running

Run the following command: `Get-Service ssh-agent`

If it is not running, use the following command to set its start type to be manual: `Set-Service -Name ssh-agent -StartupType Manual` and the following command to start it `Start-Service ssh-agent`.

## Step 4: Change Directory into the .ssh directory from the C directory

Run this command: `ssh-add id_ed25519`

You should be able to see your added identity

## Step 5: Copy the identity to clipboard

Run this command: `cat ~/.ssh/id_ed25519.pub | clip`

## Step 6: Add this key to your GitHub account

Paste this identity to Github/Settings/SSH and GPG keys/Add new SSH Key/Name it and paste the key

## Step 7: Test the connection

Run the following command: `ssh -T git@github.com`

It successful, you should see the following message: `Hi <username>! You've successfully authenticated, but GitHub does not provide shell access.
`

## Step 8: Cloning a repository

If and when you want to clone a repository using SSH, run the following command in your terminal: `git clone git@github.com:username/repository.git`
