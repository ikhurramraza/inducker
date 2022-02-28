# Inducker

Bootstraps running a docker image in current directory.

_The name "inducker" is inspired by a special kind of cricket delivery where the ball dips "in" before it reaches the batter. The default mount location is "lords" which is considered the home of cricket._

## 💿 Installation

#### Using Homebrew

```bash
brew install ikhurramraza/tap/inducker
```

## 📖 Usage

```
Usage: inducker IMAGE [OPTIONS] [-- EXTRA_ARGS]

ARGUMENTS:
  IMAGE                Docker image to use.
  EXTRA_ARGS           Extra arguments to pass to docker run.

OPTIONS:
  --directory       Which directory to mount as working directory.    Default: .
  --entrypoint      Command to launch inside the container.           Default: /bin/sh
  --mount-location  Working directory path.                           Default: /lords
```

## 🚀 Publishing

1. Create and push tag to GitHub.

```bash
git tag --sing -a "v[VERSION_TAG]" -m "[RELEASE_HEADER]"

git push origin "v[VERSION_TAG]"
```

2. Create a release on GitHub.

3. Update url and SHA in the Homebrew formula definition [here](https://github.com/ikhurramraza/homebrew-tap/blob/main/inducker.rb).

## 🤝 Contributing

Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.

## ⚖️ License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details
