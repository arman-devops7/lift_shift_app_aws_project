###### lift_shift_app_aws_project ######

# -- About the project :

# Multi Tier Web Application Stack
# Host & Run on AWS Cloud for Production
# Lift and Shift Strategy

# -- Objective :

# Flexible INFRA
# No upfront cost
# Modernize effectively
# IAAC

# -- Flow of Execution :

# Login to AWS account
# Create Key Pairs
# Launch instances with user data (Bash Scripts)
# Update IP to name mapping in route S3
# Build application from source code
# Upload to S3 Bucket
# Download artifact to Tomcat EC2 instance
# Setup ELB with HTTPS [Certificate form Amazon Certificate Manager]
# Map ELB Endpoint to website name in GoDaddy DNS
# Verify
# Build Autoscaling group for tomcat instances

# -- Architecture of aws services for the project :

# EC2 instances
# ELB
# Autoscaling
# EFS/S3 for shared storage
# Amazon Certificate manage
# Route S3

# -- AWS services used in the project :

# EC2 instances         ------- VM for Tomcat,RabbitMQ, MemCache, MySQL
# ELB (Load Balancer)   ------- NGINX LB Replacement
# Autoscaling           ------- Automation for VM scaling
# S3/EFS Storage        ------- Shared Storage
# Route S3              ------- Private DNS Service

