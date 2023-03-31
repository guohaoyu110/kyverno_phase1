# Assigned Goals

- Present proposal for phase 1 (listing all current policies in kyverno/policies on Artifact Hub)
    - Combo manual effort / script to generate AH metadata files, etc
    - Should be a complete plan with overall and detailed process




## proposal for phase 1 to list all current policies in kyverno/policies on Artifact Hub:


### Overall Process:

1. Identify the policies: Identify all the policies present in the Kyverno/policies repository that needs to be listed on Artifact Hub.
2. Generate metadata files: Generate metadata files for each policy that includes policy name, version, description, maintainers, license, and any other relevant information.
3. Create pull requests: Create pull requests to add the metadata files to the Kyverno/policies repository and submit the policies to the Artifact Hub.
4. Review and merge: Review the pull requests, and merge them once they are approved.



### Detailed Process:

#### Step 1: Identify the policies

Create a list of policies that need to be listed on the Artifact Hub. This could include all policies or a subset of policies based on certain criteria such as popularity, relevance, or maturity.

#### Step 2: Generate metadata files

2.1. For each policy, create a metadata file in the artifact-hub directory of the repository using the metadata.yaml format.

2.2. The metadata file should include the following information:
name: the name of the policy.
version: the version of the policy.
description: a brief description of the policy.
maintainers: a list of maintainers who are responsible for the policy.
license: the license under which the policy is released.
source: a URL to the source code of the policy.
keywords: a list of keywords that describe the policy.

2.3. If a policy already has a metadata file, update it with any new or changed information.

2.4. Use a script to automate the metadata file creation process as much as possible. For example, the script could parse the policy files and extract the relevant information to populate the metadata file.




#### Step 3: Create pull requests

3.1. Create a new branch for each policy metadata file: git checkout -b add-metadata/<policy-name>

3.2. Add the metadata file to the artifact-hub directory: git add artifact-hub/<policy-name>/metadata.yaml

3.3. Commit the changes: git commit -m "Add metadata for <policy-name>"

3.4. Push the changes to the remote repository: git push origin add-metadata/<policy-name>

3.5. Create a pull request on the Kyverno/policies repository to add the metadata file and submit the policy to the Artifact Hub.




#### Step 4: Review and merge

The policy will now be listed on the Artifact Hub, and users can search for and download it.
This process involves a combination of manual effort and script-based automation to generate metadata files for each policy, create pull requests to add them to the Kyverno/policies repository, and submit the policies to the Artifact Hub. By following this process, we can ensure that all current policies in Kyverno/policies are listed on the Artifact Hub, making them easily accessible to users.




