# Module 1 - Exercise 1

## Summary of Steps

1. Fork the [class GitHub repository](https://github.com/sqlity-net/dataplatform-devops-demos) to your own GitHub Account
2. Make a new feature branch called, "my-new-feature"
3. Clone the remote repository to your local machine
4. On your local machine, switch to my-new-feature
5. Open SSMS and create the tSQLt Query shortcuts
   1. Ctrl-9 → EXEC tSQLt.RunC;--
   5. Ctrl-0 → EXEC tSQLt.RunAll;--
7. In SSMS create a External Tools entry for "Build"
   1. Title → Build
   9. Command → $(ProjectDir)\build.bat
   10. Arguments → "<YOURSERVERNAME\INSTANCENAME>" "-E" **"module1demodb"**
   11. Initial directory → $(ProjectDir)
   13. Uncheck "Close on exit"
   12. Check "Use Output window"
13. Open the Module1-Exercise1 SSMS Database Solution in SSMS
14. Run Tools → Build
15. In the Object Explorer, connect to your SQL Server Instance
16. Create a new query window
17. Run "Ctrl-0" → This should result in a failing test.