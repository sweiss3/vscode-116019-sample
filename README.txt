After cloning the repository, run setup.cmd (on Windows)

This will create a directory junction from Folder2 to Client\LinkToFolder2.
Client\LinkToFolder2 is in .gitignore (as it's linking to a different place in the repository, so you don't want to have the same files twice)

Open VSCode
Navigate to Client\LinkToFolder2 and open Module2.ts

You will see the import statement is valid.
However, if you are to create a new file - Module3.ts right next to it, and add the exact same import statement - VSCode will complain that it cannot find the import.

If you restart VSCode and navigate back to Module3.ts, it will be just fine.