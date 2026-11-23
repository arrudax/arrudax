<!-- Banner -->
<h1 align="center">
  Hi, I'm Marco Arruda 👋
</h1>

<h3 align="center">
  Game Developer (Unity / C#) • Pixel Art Enthusiast
</h3>

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
