import requests

def post_files_to_discord(webhook_url, file_paths):
    for file_path in file_paths:
        with open(file_path, 'rb') as file:
            files = {'file': file}
            response = requests.post(webhook_url, files=files)
            if response.status_code == 204:
                print(f"Successfully posted {file_path}")
            else:
                print(f"Failed to post {file_path}: {response.status_code}")

if __name__ == "__main__":
    webhook_url = '#'  # Replace with your webhook URL
    file_paths = ['#', '#']    # Replace with actual file paths
    post_files_to_discord(webhook_url, file_paths)
