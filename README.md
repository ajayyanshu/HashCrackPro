# HashCrackPro

HashCrackPro is a powerful brute-force tool designed to crack MD5, SHA-1, SHA-256, and SHA-3 hashes using Python. Built for security enthusiasts and professionals, HashCrackPro leverages the power of itertools to systematically generate and test potential plaintext inputs against the target hash.

## Features

- **Multi-algorithm support**: Crack hashes generated by MD5, SHA-1, SHA-256, and SHA-3.
- **Customizable charset**: Define your own set of characters for generating potential plaintexts.
- **Adjustable length**: Set the maximum length of plaintexts to try.
- **Simple CLI**: Easy-to-use command-line interface for quick and efficient usage.

## Installation

Ensure you have Python 3 and pip installed. Install the necessary libraries using:

```sh
sudo apt-get update
sudo apt-get install python3-pip
pip3 install hashlib itertools
```

## Usage

To use HashCrackPro, clone this repository and run the script with the required parameters.

```sh
./brute_force.py <hash> <algorithm> <charset> <max_length>
```

### Parameters

- `<hash>`: The target hash you are trying to crack.
- `<algorithm>`: The hashing algorithm (md5, sha1, sha256, sha3_256).
- `<charset>`: The set of characters to use for generating potential plaintexts (e.g., `abcdefghijklmnopqrstuvwxyz`).
- `<max_length>`: The maximum length of the plaintexts to try.

### Example

To brute-force an MD5 hash using lowercase letters with a maximum length of 4:

```sh
./brute_force.py 5d41402abc4b2a76b9719d911017c592 md5 abcdefghijklmnopqrstuvwxyz 4
```

## Disclaimer

HashCrackPro is intended for educational and ethical testing purposes only. Unauthorized use of brute-force techniques can be illegal and unethical. Use this tool responsibly.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

## Contributions

Contributions are welcome! Please fork this repository and submit pull requests with your enhancements.

---