# Soundness Testnet Registration
## Link:
## https://soundness.xyz/werwewerwrw
## ➖ Submit your email

# Step 1: Generate Your Key here
```bash
sudo apt update && sudo apt upgrade -y
```

```bash
curl -sSL https://raw.githubusercontent.com/soundnesslabs/soundness-layer/main/soundnessup/install | bash
```
```bash
curl --proto '=https' --tlsv1.2 -sSf https://sh.rustup.rs/ | sh
```
```bash
source ~/.bashrc
```
```bash
soundnessup install
```
```bash
soundnessup update
```
```bash
soundness-cli generate-key --name my-key
```
## To view your seedphrase
```bash
soundness-cli list-keys
```

# Step 2: Play the Game

## ➖ Go play a game like 8queens or tictactoe.
## ➖ Once you win, the game gives you something called a proof — like a trophy.

## ➖ You’ll also get a proof file or proof blob ID (a code to prove you won).

# Step 3: Send Your Proof

**Now you can tell Soundness you won the game!**
**Here's what the command looks like:**

```bash
soundness-cli send \
--proof-file <your-proof-blob-id> \
--game <game-name> \
--key-name <your-key-name> \
--proving-system ligetron \
--payload '<json-payload>'
```
## What to fill in:

**--proof-file (-p): The unique Walrus Blob ID for your proof, which you receive after winning a game.**

**--game (-g): The name of the game you played (e.g., 8queens or tictactoe).**

**--key-name (-k): The name you chose for your key in Step 2.**

**--proving-system (-s): The ZK proving system. For our current testnet games, this is ligetron.**

**--payload (-d): A JSON string with the specific inputs required to verify your Ligetron proof.**


# Extra Commands You Might Like

 ## 1. Send a proof using local files
 
 **To send a proof and ELF Program file using local file paths:**

 ```bash
soundness-cli send --proof-file path/to/proof.proof --elf-file path/to/program.elf --key-name my-key
```
## 2. Using Files Stored as Walrus Blob IDs

**To send a proof and ELF Program file using Walrus Blob IDs (when files are already stored in Walrus):**

```bash
soundness-cli send --proof-file <proof-walrus-blob-id> --elf-file <elf-program-walrus-blob-id> --key-name my-key
```
# 3. Mixed Usage

**You can also mix file paths and Walrus Blob IDs:**

```bash
# Proof from file, ELF from Walrus storage
soundness-cli send --proof-file path/to/proof.proof --elf-file <walrus-blob-id> --key-name my-key

# Proof from Walrus storage, ELF from file  
soundness-cli send --proof-file <walrus-blob-id> --elf-file path/to/program.elf --key-name my-key
```
# 4. Proving Systems

**You can specify the proving system to use:**

```bash
soundness-cli send --proof-file <path-or-blob-id> --elf-file <path-or-blob-id> --key-name my-key --proving-system <sp1||ligetron||risc0>
```

## Supported proving systems: sp1, ligetron, risc0.

## The request will be signed using the specified key pair.

## ➖ Save your Phrase and Pub-Key
## ➖ Join Discord (https://discord.gg/soundnesslabs)
## ➖ Head to ⁠🐬│soundness-cockpit and use the /access command to submit your public key.
##✅ Done!

## Details: 
## https://x.com/SoundnessLabs/status/1902389758527152586

