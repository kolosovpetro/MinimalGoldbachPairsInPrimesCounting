# Minimal Goldbach pairs in prime and twin-prime counting

Goldbach's Conjecture assumes that every even integer $2N \geq 4$ can be written as the sum of two primes
$2N = p_i + p_j$, where $(p_i, p_j)$ is called a Goldbach pair.
The minimal Goldbach pair is a pair $(p_i, p_j)$ such that $p_i$ is minimal and $p_j = 2N - p_i$ is also a prime.
We define a function $F_{2N}(P)$ that counts the occurrences of $p_i = P$ in a set of minimal Goldbach pairs
up to $2N$, where $P$ is a fixed prime number.
In particular, the function $F_{2N}(P)$ provides the following identities in terms of prime counting $\pi(2N)$,
twin-prime counting $\pi_2(2N)$ and cousin prime counting $\pi_4(2N)$

$$\pi(2N) = F_{2N+3}(3) + 1$$
$$\pi_2(2N) = F_{2N+3}(3) - F_{2N+5}(5)$$
$$\pi_4(2N) = F_{2N}(5) - F_{2N}(7)$$


## Related MathOverflow question

- https://mathoverflow.net/q/54710/113033

## Build and run using PowerShell (Windows)

- Install `MikTeX`: https://miktex.org/download
- Update `MikTeX`
- Install `SumatraPDF` viewer: https://www.sumatrapdfreader.org/download-free-pdf-viewer
- `Rename-Tex-Files.ps1` renames main LaTeX and BibTeX files to match the repository root directory name
- `Build-Latex.ps1`

## Build and run in Intellij IDEA (Windows)

- Install `MikTeX`: https://miktex.org/download
- Update `MikTeX`
- Install `SumatraPDF` viewer: https://www.sumatrapdfreader.org/download-free-pdf-viewer
- Path to SumatraPDF: `C:\Program Files\SumatraPDF`
- Install `Intellij IDEA Ultimate`: https://www.jetbrains.com/idea/download/#section=windows
- Activate `Intellij IDEA Ultimate`
- Install `TeXiFy IDEA` plugin: https://plugins.jetbrains.com/plugin/9473-texify-idea
- Clone this repository locally: `https://github.com/kolosovpetro/github-latex-template.git`
- Open `github-latex-template` folder in `Intellij IDEA Ultimate` and configure as follows
    - LaTeX Configuration
      ![LaTeX Configuration](./src/sections/images/latex_configuration.png "LaTeX Configuration")
    - BibTeX Configuration
      ![BibTeX Configuration](./src/sections/images/bibtex_configuration.png "BibTeX Configuration")
- Configure Inverse Search in `Intellij IDEA` for SumatraPDF: `Tools -> LaTeX -> Configure Inverse Search`
- Compile document using `Shift + F10`
