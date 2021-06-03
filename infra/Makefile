up:
	terraform apply --auto-approve -var environment=${ENV}

down:
	terraform destroy --auto-approve -var environment=${ENV}

init:
	terraform init --backend-config="key=state/${ENV}.tfstate" --backend-config="dynamodb_table=RMIT-locktable-hfv6e0" --backend-config="bucket=rmit-tfstate-hfv6e0"
