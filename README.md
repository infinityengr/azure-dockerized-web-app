# Dockerized Web Application on Azure

## Overview
Built and deployed a custom Dockerized web application running on an Azure Linux virtual machine.

## Architecture
- Azure Virtual Machine (Ubuntu)
- Docker Engine
- Custom Docker image (nginx-based)
- Azure Network Security Groups (NSG)
- Public IP exposure

## What I Did
- Installed and configured Docker on an Azure VM
- Ran containerized workloads with port mapping
- Built a custom Docker image using a Dockerfile
- Deployed multiple containers on a single VM
- Configured Azure NSG rules to expose container services
- Troubleshot container and cloud networking issues

## Troubleshooting & Challenges

- Encountered external access issues when exposing Docker containers due to Azure Network Security Group (NSG) restrictions.
- Resolved by identifying required container port mappings and explicitly allowing ports 8080 and 8081 in the NSG inbound rules.
- Debugged SSH session interruptions caused by dropped connections and verified service health after reconnecting.
- Distinguished between container-level networking and cloud-level firewall configuration when diagnosing connectivity problems.

## Key Learnings
- Docker image build lifecycle
- Container port mapping vs cloud firewall rules
- Running multiple containers on a single host
- Azure VM networking and security controls

## Result
A publicly accessible, containerized web application deployed on Azure.
