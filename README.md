# Baby's First Python Code 

This project is a basic python scripts demonstrating that I have a syntax brain...

## Purpose 
Honestly, I was exhausted from YouTube programming tutorials and challenged myself to actually commit, pun-intended (more of that in a bit). So, here are some questions i asked, that may prove to be beneficial in your journey to "commit".  

This is also for if I forget how to execute any step, and don't want to accidentally hack into NASA, or your local BurgerKing. 

# What was the process like? 
1. Installing & Configuring Git on MacOS

1. Luckily I traversed down this road before so, I had already possesed a verison of git, here is the command I used to check for the installation 

      'git --version' 

2. # Setting an "identity" 
1. The sole purpose of this is to link your future commits to you 
      
      > 'git config --global user.name "Your name"' 
      > 'git config --global user.email "youremail@whatevertf.com'

      ### Tips & Best Practices 
For the email section, I recommend inserting the same email that is used for your GitHub account, the circle of the "commit life" is easier this way.
      
Think of this as when you send texts, they are linked to you through your email, or AppleID, ame thing applies here

      
3. ## Set up SSH Authentication 
1. Generating a new key 
      
      > 'ssh-keygen -t ed25519 -C "yourdesires@idk.com" 

2. Start the agent & add the key 

      > 'eval "$(ssh-agent -s)"'
      > 'ssh-add --apple-use-keychain ~/.ssh/id_ed25519'

 At this step, you may be asked to set a "passphrase".. K.I.S.S (Keep It Simple Stupid). This phrase will become your new bff, choose wisely. 

3. Copy the public key to your clipboard 

      > 'pbcopy < ~/.ssh/id_ed25519.pub'

4. Add it to GitHub --> Setting --> SSH and GPG Keys --> New SSH Key (Authentication) --> Title (Your Devices Name)

5. Test Connection In Termainal 

      > 'ssh -T git@github.com'

4. # Create a GitHub Repo (Version 01: Repository created on GitHub Website )

1. Github --> New Repository --> Name it (e.g., "hello-python-world")

2. Settings To Choose:
      
      Small written description

      Public (Open to the world) or Private (Your little secret)

      Check "Add README File" box 

      Add .gitignore (Select programming language)

      Choose a license (I chose MIT, it places few restrictions on reuse)

5. # Clone a repository locally 
1. This can be executed in your MAC OS terminal or VS Code


      > 'git clone git@github:your-username/your-project-name.git'
      > 'cd your-project-name'

You can retrieve the information that follows "git@github:" from doing the following: 
      
2. Your Repositories --> Click on it --> Code Green Button --> SSH --> Copy this link, THIS is IT GUYS, home stretch

6. # Open & Edit in VS Code
      1. Open the folder in VS Code (File --> Open)
      2. Create and edit a Python Script 
      3. Get to coding, this is YOUR time to shine

7. # Run The Program In VS Code's Terminal
      > ' python3 my_or_your_python_file.py'

8. # Version Control: Stage --> Commit --> Push

Biggest thing I've learned is that you always have to add, then commit, then push. It's just the way the programming world operates. 

1. Stage Your Edits (This is specifically for new files)
            > 'git add .'

2. Commit With a Message (Similar to a caption)

            > 'git commit -m "Message or caption/ description goes here" 

3. Push to GitHub & Feel Proud

            > ' git push'

9. ## Synopsis / Summary 
      1. **Modify** code or documents in VS Code
      2. **Run/Test** locally in your terminal
      3. **Stage/Commit** changes 
      4. **Push** to GitHub 
      5. **Verify** on GitHub.com
      6. **Rinse & Repeat**

Final Thoughts - Future README's will NEVER get this long, but somedays I have the memory of a deflated basketball, so this will come in handy. 






