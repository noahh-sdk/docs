# Setting the NOAHH_SDK environment variable

The `noahh sdk install` CLI command should automatically do this for you, however if it didn't work for some reason or you built Noahh manually, follow these instructions to set the environment variable. The variable is **required** for Noahh to work.

## On Windows

1. Search `Edit the system environment variables` on Windows search. Alternatively, you can open up Control Panel and search for it, then select `Edit the system environment variables` or **to skip straight to step 2 select `Edit environment variables for your account`**.

2. Click `Environment Variables...`

3. You can choose whether to set the variable on the User or System scope. The System scope is more likely to work but requires administrator permissions to change.

4. Click `New...` under the scope you want to create the variable for, and then name the variable `NOAHH_SDK` and make its value be the path of the Noahh repository on your computer.

![Image showing the New Environment Variable dialog on Windows](/assets/Set_Env_Var.png)

5. Press `Ok` to close the windows and then restart your computer.