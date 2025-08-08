version: 0.2
phases: 
  install: 
    runtime-versions:
      nodejs: 20
    commands:
      - npm install -g @angular/cli@17
  pre_build: 
    commands:
      - npm install
  build: 
    commands:
      - ng build -c production
    finally: 
      - echo 'This is the finally block execution!'
artifacts:
   files: 
    - appspec.yml
    - 'dist/my-angular-project/**/*'
    - 'deploy-scripts/**/*'
  