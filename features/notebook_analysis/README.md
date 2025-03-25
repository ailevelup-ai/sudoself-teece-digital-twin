# Jupyter Notebook Analysis Feature

This feature automatically generates Jupyter notebooks for each processed document in the SudoSelf Teece Digital Twin project. It provides statistical analysis, visualizations, and quality metrics to help evaluate document processing quality.

## Overview

The notebook generation feature is triggered after the Knowledge Graph Integration step in the document processing workflow. It retrieves document metadata, extracts content from S3 and DynamoDB, and generates a comprehensive notebook with the following sections:

- Document Metadata
- Text Statistical Analysis
- Entity Analysis
- Relationship Analysis
- Knowledge Graph Visualization
- Concept Distribution
- Quality Metrics
- Issues and Recommendations

## Components

- `notebook_generator_lambda.py`: Lambda function that generates the notebooks
- `requirements.txt`: Dependencies for the Lambda function
- `build_notebook_layer.sh`: Script to build the Lambda layer
- `deploy_notebook_feature.py`: Deployment script
- `notebook_feature_stack.ts`: CDK implementation
- `notebook_feature_template.yaml`: CloudFormation template

## Integration

This feature integrates with:
- SageMaker domain "sudoself" for interactive notebook access
- S3 for storing notebooks and templates
- DynamoDB for document metadata and chunks
- CloudWatch for monitoring and alerts
- Step Functions for workflow integration

## Deployment

See `deploy_notebook_feature.py` for deployment instructions.