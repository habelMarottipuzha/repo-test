# Forget your signing key????

=============================

- - - - 

 If you forget/loss your signing key what will you do?

- - - -

There are many methods to retrive or reset signing key like .jks,.keystore files.But all of them will work on file password not in certificate password(hacking certificate password is also possible,but it consumes much more time according to number of characters in the password).

There is an easy way for getting the lost/forgetton password.(This applies only if you have build application with that particular key in that particular system before.Also no logs should be cleared).
What you have to do is 
		
 Goto .AndroidStudioX.X (x.x is the version number eg 1.5) > system > log > idea in windows and open each idea.log.x file.
search for ___'android.injected.signing.store'___ and you will get something like
>	-Pandroid.injected.signing.store.file=/Users/myuserid/AndroidStudioProjects/keystore/keystore.jks, 

>	-Pandroid.injected.signing.store.password=mystorepassword, 

>	-Pandroid.injected.signing.key.alias=myandroidkeyalias, 

>	-Pandroid.injected.signing.key.password=mykeypassword,