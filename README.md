# Gitlab-Runner

# Pre-requisites
    GitLab SetUp
# GitLab SetUp
  [GitLab](https://github.com/Naresh240/Gitlab-Setup/blob/main/README.md)
# Create Project
    Open GitLab account and create new project
# Install GitLab Runner

  ![Capture](https://user-images.githubusercontent.com/54719289/104106342-f0b9f900-52da-11eb-8c40-391f3affb86b.JPG)

  Go to the project’s Settings > CI/CD and expand the Runners section and get URL and token
    
    sudo gitlab-runner register -n \
        --url http://54.144.17.106/ \
        --registration-token bszC6hSfL8fxaW4yQief \
        --executor shell \
        --description "shell-runner"
   Here We can you different executors, like shell, ssh, docker, kubernetes etc..,
 # Goto WebUI and check Runner
   Go to the project’s Settings > CI/CD and expand the Runners section
   Click on Expand
   
   ![image](https://user-images.githubusercontent.com/58024415/104083102-d0018d00-5261-11eb-8064-51d33e1de759.png)
