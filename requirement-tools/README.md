# Requirement tools
Hello dudes,   
For work with my courses, you need some requirement tools on your PC  
I will guide you how to do it  

### Windows OS
With Windows OS, a tip trick is install Git bash, and then download all binary file and copy it to git bin folder: `C:\Program Files\Git\usr\bin\`
Git-bash download: https://git-scm.com/download/win
It 's rely on your setting, please check your Git-bash setting for copy correct folder.  
 - kubectl: https://dl.k8s.io/release/v1.29.2/bin/windows/amd64/kubectl.exe
 - helm:  
 homepage: https://github.com/helm/helm/releases  
 my download: https://get.helm.sh/helm-v3.14.2-windows-amd64.zip
 - helmfile: 
 homepage: https://github.com/helmfile/helmfile/releases
 my download: https://github.com/helmfile/helmfile/releases/download/v0.162.0/helmfile_0.162.0_windows_amd64.tar.gz
 - terraform:  
 homepage: https://developer.hashicorp.com/terraform/install
 my download: https://releases.hashicorp.com/terraform/1.7.4/terraform_1.7.4_windows_amd64.zip

 
### Ubuntu OS
I don't want to using package manager, cause i am not sure where application install package,  
and because all files just a binary file, so copy to /usr/local/bin/ directory is enough
 
 - kubectl:  
 ```
 curl -LO https://dl.k8s.io/release/`curl -LS https://dl.k8s.io/release/stable.txt`/bin/linux/amd64/kubectl
 chmod +x ./kubectl
 sudo mv ./kubectl /usr/local/bin/kubectl
 kubectl version

 ```
 - helm:  
 homepage: https://github.com/helm/helm/releases  
 my download: https://get.helm.sh/helm-v3.14.2-linux-amd64.tar.gz
 - helmfile: 
 homepage: https://github.com/helmfile/helmfile/releases
 my download: https://github.com/helmfile/helmfile/releases/download/v0.162.0/helmfile_0.162.0_linux_amd64.tar.gz
 - terraform:  
 homepage: https://developer.hashicorp.com/terraform/install
 my download: https://releases.hashicorp.com/terraform/1.7.4/terraform_1.7.4_linux_amd64.zip  

 Extract all file after download and then mv all to `/usr/local/bin/` directory