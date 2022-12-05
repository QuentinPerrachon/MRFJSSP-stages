# MRFJSSP-stages

Set of instances for the MRFJSSP instances with decomposition of operation into stages

## Files format

- `5 5 25 2 2`
  - number of jobs
  - number of resources
  - total number of operations
  - max number of stages per operation
  - max number of necessary resources per operation
- **For each job :**
  - `5`
    - number of operations of each job
  - **For each operation :**
    - `2 2`
      - number of necessary resource of each operation
      - number of stages of each operation
    - **For each necessary resource :**
      - `2 2`
        - number of potential resources for each necessary resource
        - number of stages for each necessary resource
      - **For each potential resources :**
        - `5 1 8 2 7`
          - idnumber of potential resource
          - idnumber of each stages and corresponding processing times

Example above shows the beginning of the description of an instances made of 5 jobs, 5 resources, 25 operations in total, and a maximum of 2 stages and 2 necessary resources per operation.
First job has 5 operations.
First operation of the first job has 2 necessary resources and is decomposed in 2 stages.
Its first necessary resource has 2 potential resource as candidate for assignment and span over the two stages of the operation.
The first potential resource is number 5 and it has a processing time of 8 on stage 1 and a processing time of 7 on stage 2.
