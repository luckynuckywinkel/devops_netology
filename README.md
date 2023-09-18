Hello, Git!
  
---  
  
### Пояснение по файлу ./Terraform/.gitignore  
  
- В .gitignore описываются все "чувствительные" для терраформ файлы, которые могут содержать файлы конфигурации, файлы состояния инфраструктуры и переменные и которые ни коим образом не должны "светиться" в системе контроля версий.  
  
### Local .terraform directories  
  

- **/.terraform/* - игнорируются все файлы и директории, содержащиеся в директориях **.terraform** где бы они ни находились внутри проекта

### .tfstate files  
  

- *.tfstate - игнорируется <любое_имя>.tfstate  
  

- *.tfstate.* - игнорируется <любое_имя>.tfstate.<любое_расширение>  
  


### Crash log files  
  

- crash.log - игнорируется файл crash.log  
  

- crash.*.log - игнорируется любой файл файл crash.<что-то>.log  
  


### Exclude all .tfvars files, which are likely to contain sensitive data, such as
### password, private keys, and other secrets. These should not be part of version 
### control as they are data points which are potentially sensitive and subject 
### to change depending on the environment.  
  

- *.tfvars - игнорируется любой файл в формате *.tfvars  
  

- *.tfvars.json - игнорируется любой файл в формате *.tfvars.json  
  


### Ignore override files as they are usually used to override resources locally and so
### are not checked in  
  

- override.tf - игнорируется указанный файл  
  

- override.tf.json - то же самое, что и выше.  
  

- *_override.tf - игнорируется <что-либо>_override.tf  
  

- *_override.tf.json -  игнорируется <что-либо>_override.tf.json  
  


### Include override files you do wish to add to version control using negated pattern
### !example_override.tf

### Include tfplan files to ignore the plan output of command: terraform plan -out=tfplan
### example: *tfplan*

### Ignore CLI configuration files  

- .terraformrc - игнорируется скрытый файл .terraformrc  
  

- terraform.rc - игнорируется файл terraform.rc  
  

