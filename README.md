<!-- Banner -->
<h1 align="center">
  Hi, I'm Marco Arruda 👋
</h1>

<h3 align="center">
  Game Developer (Unity / C#) • Pixel Art Enthusiast
</h3>

<div align="center">
  <img src="https://github-readme-streak-stats.herokuapp.com/?user=arrudax&theme=dark&hide_border=true" alt="GitHub Streak"/>
</div>

--- 

```csharp
using System.Collections.Generic;
using UnityEngine;

public class Marco : MonoBehaviour
{
    public static Marco Instance { get; private set; }

    private void Awake()
    {
        if (Instance != null && Instance != this)
        {
            Destroy(gameObject);
            return;
        }

        Instance = this;
        DontDestroyOnLoad(gameObject);
    }

    public List<string> GetTechStack()
    {
        return new List<string>
        {
            "C",
            "C#",
            "Unity",
            "Game Development",
            "Pixel Art (WIP)"
        };
    }
}

---

<div align="center">
  <a href="https://linkedin.com/in/arrudax" target="_blank">
    <img src="https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white" alt="LinkedIn"/>
  </a>
  <a href="https://github.com/arrudax" target="_blank">
    <img src="https://img.shields.io/badge/GitHub-100000?style=for-the-badge&logo=github&logoColor=white" alt="GitHub"/>
  </a>
</div>


