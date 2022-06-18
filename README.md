# Hi 👋🏾, I'm Andre Simamora

<p><img src="https://github-readme-stats.vercel.app/api?username=andriannus&show_icons=true&theme=dark&locale=en" alt="andriannus" /></p>

## About Me

```typescript
import { useEffect, useState } from 'react';

interface CurrentWorkplace {
  company: string;
  position: string;
}

interface AboutMeState {
  currentWorkplace: CurrentWorkplace;
  dailyKnowledge: string[];
  fullName: string;
}

interface AboutMeHook {
  aboutMe: AboutMeState;
}

export default function useAboutMe(): AboutMeHook {
  const [aboutMe, setAboutMe] = useState<AboutMeState>({
    currentWorkplace: {} as CurrentWorkplace,
    dailyKnowledge: [],
    fullName: ''
  });

  useEffect(() => {
    setFullName();
    setDailyKnowledge();
    setCurrentWorkplace();
  }, []);

  function setFullName(): void {
    setAboutMe({
      ...aboutMe,
      fullName: 'Andriannus Parasian'
    });
  }

  function setCurrentWorkplace(): void {
    setAboutMe({
      ...aboutMe,
      currentWorkplace: {
        company: 'eFishery',
        position: 'Frontend Engineer'
      }
    });
  }

  function setDailyKnowledge(): void {
    setAboutMe({
      ...aboutMe,
      dailyKnowledge: [
        'JavaScript',
        'TypeScript',
        'React.js',
        'Vue',
        'Angular',
        'AJAX',
        'CSS Preprocessor',
        'Unit Test',
        'E2E Test',
        'Git',
        'JIRA/ClickUp'
      ]
    });
  }

  return { aboutMe };
}

```

### Connect with me

<p align="left">
<a href="https://bit.ly/web-andriannus" target="blank"><img align="center" src="https://cdn.jsdelivr.net/npm/simple-icons@3.0.1/icons/googlechrome.svg" alt="andriannus" height="30" width="40" /></a>
<a href="https://bit.ly/linkedin-andriannus" target="blank"><img align="center" src="https://cdn.jsdelivr.net/npm/simple-icons@3.0.1/icons/linkedin.svg" alt="andriannus" height="30" width="40" /></a>
<a href="https://bit.ly/instagram-andriannus" target="blank"><img align="center" src="https://cdn.jsdelivr.net/npm/simple-icons@3.0.1/icons/instagram.svg" alt="andriannus" height="30" width="40" /></a>
<a href="https://bit.ly/twitter-andriannus" target="blank"><img align="center" src="https://cdn.jsdelivr.net/npm/simple-icons@3.0.1/icons/twitter.svg" alt="andriannus" height="30" width="40" /></a>
<a href="https://bit.ly/facebook-andriannus" target="blank"><img align="center" src="https://cdn.jsdelivr.net/npm/simple-icons@3.0.1/icons/facebook.svg" alt="andriannus.p" height="30" width="40" /></a>
</p>
