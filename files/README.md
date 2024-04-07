## Mirroring / duplicate a repository

Open Terminal and Create a bare clone of the repository

```sh
git clone --bare https://github.com/EXAMPLE-USER/OLD-REPOSITORY.git
```

Mirror-push to the new repository

```sh
cd OLD-REPOSITORY.git
git push --mirror https://github.com/EXAMPLE-USER/NEW-REPOSITORY.git
```

Remove the temporary local repository you created earlier

```sh
cd ..
rm -rf OLD-REPOSITORY.git
```

