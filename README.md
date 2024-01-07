# Freeman instructions for becoming Humans-AI Validator

Basic server set-up security considerations:

Make sure your Fire Wall is managed all time. It is very simple matter, but represent security RISKs if not managed.

Also implement SSH key-based authentication for connecting to your Ubuntu server, you will need to install your public key on the server and configure SSH to use key-based authentication. 

1. Generate SSH Key Pair (if not already done)
First, ensure you have an SSH key pair on your local machine. If you haven't already generated one, you can do so with the following command:

sudo ssh-keygen -t ed25519

1. Set name to the new generated file when promted, so your key can be recognised in case more team members are accessing the server.
2. Set passsphrase for your keys. This will further increase protection of your server.

For people less familiarized with server management, we recommend to connect at least 2 users from diffreent machines with SSH keys before deactivating password connection in your server.  

Once your public key is installed on the server, you should be able to connect with: 

sudo ssh -i ~/.ssh/YOUR_PRIVATE_KEY USER@YOUR_SERVER_IP
