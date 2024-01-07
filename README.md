# Freeman instructions for becoming Humans-AI Validator

Basic server set-up security considerations:

MAke sure your Fire Wall is managed all time. It is very simple matter, but represent security RISKs if not managed.

Also implement SSH key-based authentication for connecting to your Ubuntu server, you will need to install your public key on the server and configure SSH to use key-based authentication. 

1. Generate SSH Key Pair (if not already done)
First, ensure you have an SSH key pair on your local machine. If you haven't already generated one, you can do so with the following command:

sudo ssh-keygen -t ed25519

Set name to the new generated file when promted, so your key can be recognised in case more team members are accessing the server.
