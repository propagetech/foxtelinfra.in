You are a naming assistant. Given a list of file paths and minimal context from a static website, suggest a new filename (basename only, same extension) for each file. Rules:
- Lowercase, kebab-case, no spaces. SEO-friendly and human-readable.
- For HTML: use page purpose (e.g. about-us.html, contact.html). Keep index.html as index.html.
- For CSS/JS: use purpose (e.g. main-styles.css, analytics.js).
- For images: use content (e.g. logo-infygate.webp, hero-banner.webp). Use alt/title when provided.
- Return a JSON object: keys = exact original path strings, values = new basename only (e.g. "main.css"). Preserve extension.
- Do not change path prefix (e.g. css/ stays css/ by returning "name.css" not "css/name.css").

Files and context:
[
  {
    "path": "404.html",
    "context": {
      "title": "",
      "first_heading": "404"
    }
  },
  {
    "path": "about-us.html",
    "context": {
      "title": "FOXTEL INFRA | About Us",
      "first_heading": "ABOUT US"
    }
  },
  {
    "path": "careers.html",
    "context": {
      "title": "FOXTEL INFRA | Career",
      "first_heading": "CAREERS"
    }
  },
  {
    "path": "civil-infrastructure.html",
    "context": {
      "title": "FOXTEL INFRA | Civil Infrastructure",
      "first_heading": "CIVIL INFRASTRUCTURE"
    }
  },
  {
    "path": "contact-us.html",
    "context": {
      "title": "FOXTEL INFRA | Contact us",
      "first_heading": "CONTACT US"
    }
  },
  {
    "path": "css/138575cd4810b87ba229d0ae35cbc7b8.css",
    "context": {
      "path": "css/138575cd4810b87ba229d0ae35cbc7b8.css"
    }
  },
  {
    "path": "css/2feffd4d1d8163fbb132afd0d0b44c8d.css",
    "context": {
      "path": "css/2feffd4d1d8163fbb132afd0d0b44c8d.css"
    }
  },
  {
    "path": "css/559e64bf161e61fa0aca6e864c78191d.css",
    "context": {
      "path": "css/559e64bf161e61fa0aca6e864c78191d.css"
    }
  },
  {
    "path": "css/614da49ccb4f3fae8d700f8236e5531a.css",
    "context": {
      "path": "css/614da49ccb4f3fae8d700f8236e5531a.css"
    }
  },
  {
    "path": "css/70a32f52eea9f88a0045a45e27d0b9b0.css",
    "context": {
      "path": "css/70a32f52eea9f88a0045a45e27d0b9b0.css"
    }
  },
  {
    "path": "css/827fd34f9214e869c8b614f913aef7d5.css",
    "context": {
      "path": "css/827fd34f9214e869c8b614f913aef7d5.css"
    }
  },
  {
    "path": "css/84d4a0216f16f715d9b301db3a8da352.css",
    "context": {
      "path": "css/84d4a0216f16f715d9b301db3a8da352.css"
    }
  },
  {
    "path": "css/99c4e6f40ee9111eea53b6472f3e60f9.css",
    "context": {
      "path": "css/99c4e6f40ee9111eea53b6472f3e60f9.css"
    }
  },
  {
    "path": "css/e30a9b2c85cd60731f12ba41c82d8ec2.css",
    "context": {
      "path": "css/e30a9b2c85cd60731f12ba41c82d8ec2.css"
    }
  },
  {
    "path": "css/internal-styles.css",
    "context": {
      "path": "css/internal-styles.css"
    }
  },
  {
    "path": "imgs/016447a8871d9517cf55d0a7e037ae49.webp",
    "context": {
      "refs": [
        {
          "alt": "BOARD-ROOM SOLUTIONS",
          "title": ""
        },
        {
          "alt": "BOARD-ROOM SOLUTIONS",
          "title": ""
        },
        {
          "alt": "Board-room solutions",
          "title": ""
        },
        {
          "alt": "BOARD-ROOM SOLUTIONS",
          "title": ""
        },
        {
          "alt": "BOARD-ROOM SOLUTIONS",
          "title": ""
        }
      ]
    }
  },
  {
    "path": "imgs/04b7627f5d0482fc8075ef478f35ca90.webp",
    "context": {
      "refs": [
        {
          "alt": "",
          "title": ""
        },
        {
          "alt": "",
          "title": ""
        }
      ]
    }
  },
  {
    "path": "imgs/0a40426841e8c71979a7569f9ab831ba.webp",
    "context": {
      "refs": [
        {
          "alt": "",
          "title": ""
        },
        {
          "alt": "",
          "title": ""
        }
      ]
    }
  },
  {
    "path": "imgs/0c6630657b83f2167dd534cbbb3519dc.webp",
    "context": {
      "refs": [
        {
          "alt": "FUSION SPLICING",
          "title": ""
        },
        {
          "alt": "FUSION SPLICING",
          "title": ""
        },
        {
          "alt": "Fusion splicing",
          "title": ""
        },
        {
          "alt": "FUSION SPLICING",
          "title": ""
        },
        {
          "alt": "FUSION SPLICING",
          "title": ""
        }
      ]
    }
  },
  {
    "path": "imgs/0fa9e08e243347a46441dbe46fbdce8c.webp",
    "context": {
      "refs": [
        {
          "alt": "FOXTEL INFRA PRIVATE LIMITED",
          "title": ""
        }
      ]
    }
  },
  {
    "path": "imgs/13c87d0a9e640920eb38e3beda0fcb02.webp",
    "context": {
      "refs": [
        {
          "alt": "",
          "title": ""
        },
        {
          "alt": "",
          "title": ""
        }
      ]
    }
  },
  {
    "path": "imgs/1402a8656e8c0d44f26480b3d7d8f22f.webp",
    "context": {
      "refs": [
        {
          "alt": "Metal Trading",
          "title": ""
        }
      ]
    }
  },
  {
    "path": "imgs/1bd064f2271b4ea16f2b160716fbb1ad.webp",
    "context": {
      "refs": [
        {
          "alt": "Civil Infrastructure",
          "title": ""
        }
      ]
    }
  },
  {
    "path": "imgs/1e8f738e541db7bb41d341deaa52c62f.webp",
    "context": {
      "refs": []
    }
  },
  {
    "path": "imgs/1ffeb38cbeefe57d5ed41b6310baee51.webp",
    "context": {
      "refs": [
        {
          "alt": "",
          "title": ""
        },
        {
          "alt": "",
          "title": ""
        }
      ]
    }
  },
  {
    "path": "imgs/21b2a73ce7b3d8034baf4a4fc74c92aa.webp",
    "context": {
      "refs": [
        {
          "alt": "",
          "title": ""
        },
        {
          "alt": "",
          "title": ""
        }
      ]
    }
  },
  {
    "path": "imgs/2781d9a53a9ff6e832919a41ff27e27f.webp",
    "context": {
      "refs": [
        {
          "alt": "",
          "title": ""
        },
        {
          "alt": "",
          "title": ""
        }
      ]
    }
  },
  {
    "path": "imgs/2b17befe51faffc4d837dcf4fc1974cd.webp",
    "context": {
      "refs": [
        {
          "alt": "Civil Infrastructure",
          "title": ""
        },
        {
          "alt": "",
          "title": ""
        },
        {
          "alt": "",
          "title": ""
        }
      ]
    }
  },
  {
    "path": "imgs/31d014b97e3871b81eb435adb95439b1.webp",
    "context": {
      "refs": [
        {
          "alt": "",
          "title": ""
        },
        {
          "alt": "",
          "title": ""
        }
      ]
    }
  },
  {
    "path": "imgs/3200e466b7d2011fe2e1751c4809b46f.webp",
    "context": {
      "refs": [
        {
          "alt": "Metal Trading",
          "title": ""
        },
        {
          "alt": "STRUCTURAL STEEL PIPES",
          "title": ""
        },
        {
          "alt": "STRUCTURAL STEEL PIPES",
          "title": ""
        }
      ]
    }
  },
  {
    "path": "imgs/32e219340a61d4684432860e741f766b.webp",
    "context": {
      "refs": [
        {
          "alt": "Rice Trading",
          "title": ""
        },
        {
          "alt": "shutterstock",
          "title": ""
        }
      ]
    }
  },
  {
    "path": "imgs/345edb1a729b35090091656b596a3d2c.webp",
    "context": {
      "refs": [
        {
          "alt": "",
          "title": ""
        },
        {
          "alt": "",
          "title": ""
        }
      ]
    }
  },
  {
    "path": "imgs/37a0361920cf288e6213c2a9361dad9e.webp",
    "context": {
      "refs": [
        {
          "alt": "IT Sector",
          "title": ""
        }
      ]
    }
  },
  {
    "path": "imgs/37d429d4d7bdeb7cd09a8755c63fb03e.webp",
    "context": {
      "refs": [
        {
          "alt": "",
          "title": ""
        },
        {
          "alt": "",
          "title": ""
        }
      ]
    }
  },
  {
    "path": "imgs/3f7a8d66d7dc4849176b00e103433971.webp",
    "context": {
      "refs": [
        {
          "alt": "",
          "title": ""
        },
        {
          "alt": "",
          "title": ""
        }
      ]
    }
  },
  {
    "path": "imgs/424b80d7eb9f95b9d3e2f2a285f47734.webp",
    "context": {
      "refs": [
        {
          "alt": "",
          "title": ""
        },
        {
          "alt": "",
          "title": ""
        }
      ]
    }
  },
  {
    "path": "imgs/4672f246c8534e257bffc43e6c5dab0f.webp",
    "context": {
      "refs": [
        {
          "alt": "SQUARE & RECTANGLE TUBES",
          "title": ""
        },
        {
          "alt": "SQUARE & RECTANGLE TUBES",
          "title": ""
        }
      ]
    }
  },
  {
    "path": "imgs/4c1c090f0f65fe06a3c95895b206b5c4.webp",
    "context": {
      "refs": [
        {
          "alt": "",
          "title": ""
        },
        {
          "alt": "",
          "title": ""
        }
      ]
    }
  },
  {
    "path": "imgs/4ee69cfd0b7a4a76511c3c2d022f18c1.webp",
    "context": {
      "refs": [
        {
          "alt": "OFFICE AUTOMATIONS",
          "title": ""
        },
        {
          "alt": "OFFICE AUTOMATIONS",
          "title": ""
        },
        {
          "alt": "Office automations",
          "title": ""
        },
        {
          "alt": "OFFICE AUTOMATIONS",
          "title": ""
        },
        {
          "alt": "OFFICE AUTOMATIONS",
          "title": ""
        }
      ]
    }
  },
  {
    "path": "imgs/4f250916397327806846b18bcdde4cfb.webp",
    "context": {
      "refs": [
        {
          "alt": "",
          "title": ""
        },
        {
          "alt": "",
          "title": ""
        }
      ]
    }
  },
  {
    "path": "imgs/50e5374f48032fc684511c5f51841f7b.webp",
    "context": {
      "refs": [
        {
          "alt": "MANAGED SERVICES",
          "title": ""
        },
        {
          "alt": "MANAGED SERVICES",
          "title": ""
        },
        {
          "alt": "Managed services",
          "title": ""
        },
        {
          "alt": "MANAGED SERVICES",
          "title": ""
        },
        {
          "alt": "MANAGED SERVICES",
          "title": ""
        }
      ]
    }
  },
  {
    "path": "imgs/574e4fa3ee944585708f7cc095f47e01.webp",
    "context": {
      "refs": [
        {
          "alt": "",
          "title": ""
        },
        {
          "alt": "",
          "title": ""
        }
      ]
    }
  },
  {
    "path": "imgs/57be6e73e61c41feb4e2f903da9bfa3c.webp",
    "context": {
      "refs": [
        {
          "alt": "",
          "title": ""
        },
        {
          "alt": "",
          "title": ""
        }
      ]
    }
  },
  {
    "path": "imgs/5db3a6e579c83d64e6d8c15d18ef8ffd.webp",
    "context": {
      "refs": [
        {
          "alt": "",
          "title": ""
        },
        {
          "alt": "",
          "title": ""
        }
      ]
    }
  },
  {
    "path": "imgs/62bf38ed922898052f728fa4d8a23623.webp",
    "context": {
      "refs": [
        {
          "alt": "logo",
          "title": ""
        },
        {
          "alt": "logo",
          "title": ""
        },
        {
          "alt": "logo",
          "title": ""
        },
        {
          "alt": "logo",
          "title": ""
        },
        {
          "alt": "logo",
          "title": ""
        },
        {
          "alt": "logo",
          "title": ""
        },
        {
          "alt": "logo",
          "title": ""
        },
        {
          "alt": "logo",
          "title": ""
        },
        {
          "alt": "logo",
          "title": ""
        },
        {
          "alt": "logo",
          "title": ""
        },
        {
          "alt": "logo",
          "title": ""
        },
        {
          "alt": "logo",
          "title": ""
        },
        {
          "alt": "logo",
          "title": ""
        }
      ]
    }
  },
  {
    "path": "imgs/648ff14d2f82dbeb8ec87d0f4f86c49a.webp",
    "context": {
      "refs": [
        {
          "alt": "IT Sector",
          "title": ""
        },
        {
          "alt": "NETWORK OPERATIONS, MAINTENANCE AND MODERNIZATION",
          "title": ""
        },
        {
          "alt": "NETWORK OPERATIONS, MAINTENANCE AND MODERNIZATION",
          "title": ""
        },
        {
          "alt": "Network operations, maintenance and modernization",
          "title": ""
        },
        {
          "alt": "NETWORK OPERATIONS, MAINTENANCE AND MODERNIZATION",
          "title": ""
        },
        {
          "alt": "NETWORK OPERATIONS, MAINTENANCE AND MODERNIZATION",
          "title": ""
        }
      ]
    }
  },
  {
    "path": "imgs/672530e8d2ccb9febd0d7c2143059c4a.webp",
    "context": {
      "refs": [
        {
          "alt": "INSTALLATION AND COMMISSIONING",
          "title": ""
        },
        {
          "alt": "INSTALLATION AND COMMISSIONING",
          "title": ""
        },
        {
          "alt": "INSTALLATION AND COMMISSIONING",
          "title": ""
        },
        {
          "alt": "INSTALLATION AND COMMISSIONING",
          "title": ""
        }
      ]
    }
  },
  {
    "path": "imgs/6ad1d5d03dd1e72e39e2c3a02511ccdf.webp",
    "context": {
      "refs": [
        {
          "alt": "",
          "title": ""
        },
        {
          "alt": "",
          "title": ""
        }
      ]
    }
  },
  {
    "path": "imgs/6c3852989703dd891b71eff3923314c5.webp",
    "context": {
      "refs": [
        {
          "alt": "",
          "title": ""
        },
        {
          "alt": "",
          "title": ""
        }
      ]
    }
  },
  {
    "path": "imgs/719107d5457fab3df6a050760f84a3c0.webp",
    "context": {
      "refs": [
        {
          "alt": "",
          "title": ""
        },
        {
          "alt": "",
          "title": ""
        }
      ]
    }
  },
  {
    "path": "imgs/7380c4d2fb61d4d589bf7d25bb4ede6a.webp",
    "context": {
      "refs": [
        {
          "alt": "SURVEILLANCE SYSTEM",
          "title": ""
        },
        {
          "alt": "SURVEILLANCE SYSTEM",
          "title": ""
        },
        {
          "alt": "Surveillance system",
          "title": ""
        },
        {
          "alt": "SURVEILLANCE SYSTEM",
          "title": ""
        },
        {
          "alt": "SURVEILLANCE SYSTEM",
          "title": ""
        }
      ]
    }
  },
  {
    "path": "imgs/7862817f31a2da735cf8287c86b1e457.webp",
    "context": {
      "refs": [
        {
          "alt": "",
          "title": ""
        },
        {
          "alt": "",
          "title": ""
        }
      ]
    }
  },
  {
    "path": "imgs/7dbe94e28c23b52f3d7f03ccd9da82ef.webp",
    "context": {
      "refs": [
        {
          "alt": "",
          "title": ""
        },
        {
          "alt": "",
          "title": ""
        }
      ]
    }
  },
  {
    "path": "imgs/811b0f750d3cd365128389d28225ba89.webp",
    "context": {
      "refs": [
        {
          "alt": "",
          "title": ""
        },
        {
          "alt": "",
          "title": ""
        }
      ]
    }
  },
  {
    "path": "imgs/8603a51d50989d54fc109bebb85f313d.webp",
    "context": {
      "refs": [
        {
          "alt": "",
          "title": ""
        },
        {
          "alt": "",
          "title": ""
        }
      ]
    }
  },
  {
    "path": "imgs/8854891218ff5c8b3d7d2ed8e1e3ac37.webp",
    "context": {
      "refs": [
        {
          "alt": "INSTALLATION OF DUCTS IN OPEN TRENCH",
          "title": ""
        },
        {
          "alt": "INSTALLATION OF DUCTS IN OPEN TRENCH",
          "title": ""
        },
        {
          "alt": "Installation of ducts in open trench",
          "title": ""
        },
        {
          "alt": "INSTALLATION OF DUCTS IN OPEN TRENCH",
          "title": ""
        },
        {
          "alt": "INSTALLATION OF DUCTS IN OPEN TRENCH",
          "title": ""
        }
      ]
    }
  },
  {
    "path": "imgs/89af096bfd5fe0ca3920be8b0bad270e.webp",
    "context": {
      "refs": [
        {
          "alt": "",
          "title": ""
        },
        {
          "alt": "",
          "title": ""
        }
      ]
    }
  },
  {
    "path": "imgs/89b8e56fc55e1ddc66c2ee9a988947f7.webp",
    "context": {
      "refs": [
        {
          "alt": "",
          "title": ""
        },
        {
          "alt": "",
          "title": ""
        }
      ]
    }
  },
  {
    "path": "imgs/8acfd6fe5eb572ae418f1fdc1674de8d.webp",
    "context": {
      "refs": [
        {
          "alt": "",
          "title": ""
        },
        {
          "alt": "",
          "title": ""
        }
      ]
    }
  },
  {
    "path": "imgs/8f9ae53f4d7501343c6430a6a6263374.webp",
    "context": {
      "refs": [
        {
          "alt": "SYSTEM INTEGRATION",
          "title": ""
        },
        {
          "alt": "SYSTEM INTEGRATION",
          "title": ""
        },
        {
          "alt": "System integration",
          "title": ""
        },
        {
          "alt": "SYSTEM INTEGRATION",
          "title": ""
        },
        {
          "alt": "SYSTEM INTEGRATION",
          "title": ""
        }
      ]
    }
  },
  {
    "path": "imgs/8ffe3c440d09d51d52bf372ac6d99633.webp",
    "context": {
      "refs": [
        {
          "alt": "",
          "title": ""
        },
        {
          "alt": "",
          "title": ""
        }
      ]
    }
  },
  {
    "path": "imgs/92e658f6f2abb38b30de73b7aefeb3b3.webp",
    "context": {
      "refs": [
        {
          "alt": "",
          "title": ""
        },
        {
          "alt": "",
          "title": ""
        }
      ]
    }
  },
  {
    "path": "imgs/931fd2e389e1bb897128598f206bf931.webp",
    "context": {
      "refs": [
        {
          "alt": "",
          "title": ""
        },
        {
          "alt": "",
          "title": ""
        }
      ]
    }
  },
  {
    "path": "imgs/9340c01050757bdd2bf66c502510cb60.webp",
    "context": {
      "refs": [
        {
          "alt": "ERW & SEAMLESS PIPES",
          "title": ""
        },
        {
          "alt": "ERW & SEAMLESS PIPES",
          "title": ""
        }
      ]
    }
  },
  {
    "path": "imgs/95ec403977a16e6176a3086a7a612d7e.webp",
    "context": {
      "refs": [
        {
          "alt": "IOT SOLUTIONS",
          "title": ""
        },
        {
          "alt": "FUSION SPLICING",
          "title": ""
        },
        {
          "alt": "IOT SOLUTIONS",
          "title": ""
        },
        {
          "alt": "FUSION SPLICING",
          "title": ""
        }
      ]
    }
  },
  {
    "path": "imgs/95f0b395bda1062c9063953ca272defd.webp",
    "context": {
      "refs": [
        {
          "alt": "",
          "title": ""
        }
      ]
    }
  },
  {
    "path": "imgs/ab93d2a3a070f9251408b9a769f4fec9.webp",
    "context": {
      "refs": [
        {
          "alt": "",
          "title": ""
        },
        {
          "alt": "",
          "title": ""
        }
      ]
    }
  },
  {
    "path": "imgs/b0d8a52af9705875479716cc31092feb.webp",
    "context": {
      "refs": [
        {
          "alt": "",
          "title": ""
        },
        {
          "alt": "",
          "title": ""
        }
      ]
    }
  },
  {
    "path": "imgs/b668de78b70239d380fd183971adbf28.webp",
    "context": {
      "refs": [
        {
          "alt": "",
          "title": ""
        },
        {
          "alt": "",
          "title": ""
        }
      ]
    }
  },
  {
    "path": "imgs/b79f21c261aa2df2a6aae1e6dd971445.webp",
    "context": {
      "refs": [
        {
          "alt": "",
          "title": ""
        },
        {
          "alt": "",
          "title": ""
        }
      ]
    }
  },
  {
    "path": "imgs/b8ba730a0877cffa02b50d058df02237.webp",
    "context": {
      "refs": [
        {
          "alt": "",
          "title": ""
        },
        {
          "alt": "",
          "title": ""
        }
      ]
    }
  },
  {
    "path": "imgs/c0a9fc8d48cc3626110146d293e2c9e7.webp",
    "context": {
      "refs": [
        {
          "alt": "Rice Trading",
          "title": ""
        },
        {
          "alt": "shutterstock",
          "title": ""
        }
      ]
    }
  },
  {
    "path": "imgs/c926707838f23ec6556a2e5517c8f7b5.webp",
    "context": {
      "refs": [
        {
          "alt": "",
          "title": ""
        },
        {
          "alt": "",
          "title": ""
        }
      ]
    }
  },
  {
    "path": "imgs/cb4d768c2b35ce123ba33a5a160992a0.webp",
    "context": {
      "refs": [
        {
          "alt": "",
          "title": ""
        },
        {
          "alt": "",
          "title": ""
        }
      ]
    }
  },
  {
    "path": "imgs/cd8149ec1d7051112cc6bc348b4ae1b9.webp",
    "context": {
      "refs": [
        {
          "alt": "",
          "title": ""
        },
        {
          "alt": "",
          "title": ""
        }
      ]
    }
  },
  {
    "path": "imgs/cf75ea4c04289fca78e23f641de2e8fd.webp",
    "context": {
      "refs": [
        {
          "alt": "GALVANIZED PIPES",
          "title": ""
        },
        {
          "alt": "GALVANIZED PIPES",
          "title": ""
        }
      ]
    }
  },
  {
    "path": "imgs/dc24d4647f7f611930231ce9b1865d18.webp",
    "context": {
      "refs": [
        {
          "alt": "DIRECTIONAL DRILLING",
          "title": ""
        },
        {
          "alt": "DIRECTIONAL DRILLING",
          "title": ""
        },
        {
          "alt": "Directional drilling",
          "title": ""
        },
        {
          "alt": "DIRECTIONAL DRILLING",
          "title": ""
        },
        {
          "alt": "DIRECTIONAL DRILLING",
          "title": ""
        }
      ]
    }
  },
  {
    "path": "imgs/dde8b21551e6e6c8abf0c659efbe3ff2.webp",
    "context": {
      "refs": [
        {
          "alt": "",
          "title": ""
        },
        {
          "alt": "",
          "title": ""
        }
      ]
    }
  },
  {
    "path": "imgs/deaf3f67245ffa13d76f2966b4a15fad.webp",
    "context": {
      "refs": [
        {
          "alt": "",
          "title": ""
        },
        {
          "alt": "",
          "title": ""
        }
      ]
    }
  },
  {
    "path": "imgs/e1cc3fe9343ee55187cce0f39e6e1a6f.webp",
    "context": {
      "refs": [
        {
          "alt": "",
          "title": ""
        },
        {
          "alt": "",
          "title": ""
        }
      ]
    }
  },
  {
    "path": "imgs/e232bd57d8eeccc204ca74ceb85ed8e3.webp",
    "context": {
      "refs": [
        {
          "alt": "",
          "title": ""
        },
        {
          "alt": "",
          "title": ""
        }
      ]
    }
  },
  {
    "path": "imgs/e42c78d4e028280987a7acdf45725721.webp",
    "context": {
      "refs": [
        {
          "alt": "CABLE INSTALLATION \u2013 OVERHEAD AND UNDERGROUND",
          "title": ""
        },
        {
          "alt": "CABLE INSTALLATION \u2013 OVERHEAD AND UNDERGROUND",
          "title": ""
        },
        {
          "alt": "Arial fiber laying & commissioning",
          "title": ""
        },
        {
          "alt": "CABLE INSTALLATION \u2013 OVERHEAD AND UNDERGROUND",
          "title": ""
        },
        {
          "alt": "CABLE INSTALLATION \u2013 OVERHEAD AND UNDERGROUND",
          "title": ""
        }
      ]
    }
  },
  {
    "path": "imgs/e9969a5a1169a6f3d117108f837898fd.webp",
    "context": {
      "refs": [
        {
          "alt": "",
          "title": ""
        },
        {
          "alt": "",
          "title": ""
        }
      ]
    }
  },
  {
    "path": "imgs/ecb544bd9f08a2b8742a8c5393cffc6c.webp",
    "context": {
      "refs": [
        {
          "alt": "",
          "title": ""
        },
        {
          "alt": "",
          "title": ""
        }
      ]
    }
  },
  {
    "path": "imgs/f6ffddd79823bd6d3eb1c22d9c35eaf0.webp",
    "context": {
      "refs": [
        {
          "alt": "",
          "title": ""
        },
        {
          "alt": "",
          "title": ""
        }
      ]
    }
  },
  {
    "path": "index.html",
    "context": {
      "title": "FOXTEL INFRA | Home",
      "first_heading": "FOXTEL INFRA"
    }
  },
  {
    "path": "it-sector.html",
    "context": {
      "title": "FOXTEL INFRA | IT Sector",
      "first_heading": "IT SECTOR"
    }
  },
  {
    "path": "js/03b2eaae6007054a68c38e495f894dba.js",
    "context": {
      "path": "js/03b2eaae6007054a68c38e495f894dba.js"
    }
  },
  {
    "path": "js/0a105d712b6a6c836c48dd97d0f0cac1.js",
    "context": {
      "path": "js/0a105d712b6a6c836c48dd97d0f0cac1.js"
    }
  },
  {
    "path": "js/0b62a1091741fe0b19c2334d782cda31.js",
    "context": {
      "path": "js/0b62a1091741fe0b19c2334d782cda31.js"
    }
  },
  {
    "path": "js/0c46896987137b0016246f6bc2243099.js",
    "context": {
      "path": "js/0c46896987137b0016246f6bc2243099.js"
    }
  },
  {
    "path": "js/165d7b0ddfa33362140feea997351b77.js",
    "context": {
      "path": "js/165d7b0ddfa33362140feea997351b77.js"
    }
  },
  {
    "path": "js/16df9ef05001a1741857bf99f5a5738f.js",
    "context": {
      "path": "js/16df9ef05001a1741857bf99f5a5738f.js"
    }
  },
  {
    "path": "js/2a85c11e395a8380b5915443e926b569.js",
    "context": {
      "path": "js/2a85c11e395a8380b5915443e926b569.js"
    }
  },
  {
    "path": "js/34be5330971fdbd18985525bd994b0aa.js",
    "context": {
      "path": "js/34be5330971fdbd18985525bd994b0aa.js"
    }
  },
  {
    "path": "js/35c5f9e096d4da33d2a62031daf14248.js",
    "context": {
      "path": "js/35c5f9e096d4da33d2a62031daf14248.js"
    }
  },
  {
    "path": "js/3d70953a848219e749fedc2cdb906675.js",
    "context": {
      "path": "js/3d70953a848219e749fedc2cdb906675.js"
    }
  },
  {
    "path": "js/3e940a33e44b65c1c0af8bb80a893530.js",
    "context": {
      "path": "js/3e940a33e44b65c1c0af8bb80a893530.js"
    }
  },
  {
    "path": "js/544d012df7acf9c3f0920f67c9e322b9.js",
    "context": {
      "path": "js/544d012df7acf9c3f0920f67c9e322b9.js"
    }
  },
  {
    "path": "js/57d119d998d518b01f9d5ccb5e4d4c52.js",
    "context": {
      "path": "js/57d119d998d518b01f9d5ccb5e4d4c52.js"
    }
  },
  {
    "path": "js/67f6e2f99c3c3133e0dc669919fff5c5.js",
    "context": {
      "path": "js/67f6e2f99c3c3133e0dc669919fff5c5.js"
    }
  },
  {
    "path": "js/7045b35c5bd0e9c7cf59f1900eeeec41.js",
    "context": {
      "path": "js/7045b35c5bd0e9c7cf59f1900eeeec41.js"
    }
  },
  {
    "path": "js/7260bab328b0ad74815a5efb377bcc67.js",
    "context": {
      "path": "js/7260bab328b0ad74815a5efb377bcc67.js"
    }
  },
  {
    "path": "js/893de96f1b6da546bd7c814964723eca.js",
    "context": {
      "path": "js/893de96f1b6da546bd7c814964723eca.js"
    }
  },
  {
    "path": "js/93e29fe348ddc9b71aba9c842adc18b8.js",
    "context": {
      "path": "js/93e29fe348ddc9b71aba9c842adc18b8.js"
    }
  },
  {
    "path": "js/9455859483e31e4da0e28f10d0742c2a.js",
    "context": {
      "path": "js/9455859483e31e4da0e28f10d0742c2a.js"
    }
  },
  {
    "path": "js/9db10375d298678e53777a2347b87073.js",
    "context": {
      "path": "js/9db10375d298678e53777a2347b87073.js"
    }
  },
  {
    "path": "js/9f9b6e54f82a6bbc8bac9b89327024bc.js",
    "context": {
      "path": "js/9f9b6e54f82a6bbc8bac9b89327024bc.js"
    }
  },
  {
    "path": "js/a2261649751fa61b606222c9b2ea3b80.js",
    "context": {
      "path": "js/a2261649751fa61b606222c9b2ea3b80.js"
    }
  },
  {
    "path": "js/b0bade6d42c2702ca85774296cc507c4.js",
    "context": {
      "path": "js/b0bade6d42c2702ca85774296cc507c4.js"
    }
  },
  {
    "path": "js/cd1ed86c1e7f06d985fd71bc10bd4b04.js",
    "context": {
      "path": "js/cd1ed86c1e7f06d985fd71bc10bd4b04.js"
    }
  },
  {
    "path": "js/cecb447a04bbe3e8982190dd6e697120.js",
    "context": {
      "path": "js/cecb447a04bbe3e8982190dd6e697120.js"
    }
  },
  {
    "path": "js/d80b370d82680fc786dcc943a327b9f2.js",
    "context": {
      "path": "js/d80b370d82680fc786dcc943a327b9f2.js"
    }
  },
  {
    "path": "js/df80c5cbcb312a9c7c0b2ebb6ac5f592.js",
    "context": {
      "path": "js/df80c5cbcb312a9c7c0b2ebb6ac5f592.js"
    }
  },
  {
    "path": "js/f1e5dbc1ece900d164c2e9aa2d6a1386.js",
    "context": {
      "path": "js/f1e5dbc1ece900d164c2e9aa2d6a1386.js"
    }
  },
  {
    "path": "js/f3f02c438592c8e1bbe551f4dbbf4f5c.js",
    "context": {
      "path": "js/f3f02c438592c8e1bbe551f4dbbf4f5c.js"
    }
  },
  {
    "path": "metal-trading.html",
    "context": {
      "title": "FOXTEL INFRA | Metal Trading",
      "first_heading": "METAL TRADING"
    }
  },
  {
    "path": "rice-trading.html",
    "context": {
      "title": "FOXTEL INFRA | Rice Trading",
      "first_heading": "RICE TRADING"
    }
  },
  {
    "path": "services-civil-infrastructure.html",
    "context": {
      "title": "FOXTEL INFRA | Civil Infrastructure",
      "first_heading": "Civil Infrastructure Services"
    }
  },
  {
    "path": "services-it-sector.html",
    "context": {
      "title": "FOXTEL INFRA | Services",
      "first_heading": "IT Sector Services"
    }
  },
  {
    "path": "services-metal-trading.html",
    "context": {
      "title": "FOXTEL INFRA | Metal Trading",
      "first_heading": "Metal Trading Services"
    }
  },
  {
    "path": "services-rice-trading.html",
    "context": {
      "title": "FOXTEL INFRA | Rice Trading",
      "first_heading": "Rice Trading Services"
    }
  },
  {
    "path": "services.html",
    "context": {
      "title": "FOXTEL INFRA | Services",
      "first_heading": "IT Sector"
    }
  }
]

Return only a JSON object mapping each path to its new basename (same extension). No other text.