Step 1:
- Create the Project Directory or Repository:

```bash
mkdir <project_directory_name> && cd <project_directory_name>
```

OR

```bash
git clone <repo_url>
cd <repo_name>
```

*ArtMe* is the Project Directory or Repository which would contain the project's
root folder. Create and Enter into the directory or repository.

Step 2:
- Generate the ASP.NET Core Web API Project:

```bash
docker run --rm -v $(pwd):/app -w /app mcr.microsoft.com/dotnet/sdk:9.0 dotnet new webapi -o <name_of_project>
```
In our case:

```bash
docker run --rm -v $(pwd):/app -w /app mcr.microsoft.com/dotnet/sdk:9.0 dotnet new webapi -o ArtMeAPI
```

Step 3:
- Change ownership of the project directory created on your local host machine to make edits to the files in it.

```bash
sudo chown -R $USER ArtMeAPI
```

- Navigate to the Project Directory:

```bash
cd ArtMeAPI
```

Step 4:
- Create a new directory for storing schemas called `Models`

```bash
mkdir Models
'''

- Navigate into ```Models```

```bash
cd Models
```
