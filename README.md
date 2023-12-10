# happydev-chatapp
feature branch test

Changed Readme

-Changed/hardcoded ECS cluster directory to environments/feature 
    line 92 
        # Use Terraform to create AWS ECS resources like cluster, task definition, and service
      - name: Create AWS ECS cluster, task definition and service using Terraform
        id: terraform-ecs # Define an id which allows other steps to reference outputs from this step.
        working-directory: ./environments/feature  # Set the working directory for this step
-Changed/hardcoded directory for terraform output
 # Retrieve the access URL from Terraform outputs
      - name: Set up Terraform outputs
        id: tf-outputs  # Define an id for this step to be used in the subsequent steps.
        working-directory: ./environments/feature  # Set the working directory for this step