# Hi 👋🏾, I'm Andre Simamora

<p><img src="https://github-readme-stats.vercel.app/api?username=andriannus&show_icons=true&theme=dark&locale=en" alt="andriannus" /></p>

## About Me

```typescript
import { useCallback, useEffect, useState } from 'react';

type CurrentWorkplace = {
  company: string;
  position: string;
}

type AboutMeState = {
  currentWorkplace: Partial<CurrentWorkplace>;
  fullName: string;
  skills: string[];
}

type UseAboutMe = {
  aboutMe: AboutMeState;
}

export function useAboutMe(): UseAboutMe {
  const [aboutMe, setAboutMe] = useState<AboutMeState>({
    currentWorkplace: {},
    fullName: ''
    skills: [],
  });

  const setFullName = useCallback(() => {
    setAboutMe((prevState) => ({
      ...prevState,
      fullName: 'Andriannus Parasian'
    }));
  }, []);

  const setCurrentWorkplace = useCallback(() => {
    setAboutMe((prevState) => ({
      ...prevState,
      currentWorkplace: {
        company: 'N/A',
        position: 'N/A'
      }
    }));
  }, []);

  const setSkills = useCallback(() => {
    setAboutMe((prevState) => ({
      ...prevState,
      skills: [
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
    }));
  }, []);

  useEffect(() => {
    setFullName();
    setCurrentWorkplace();
    setSkills();
  }, [setFullName, setCurrentWorkplace, setSkills]);

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
