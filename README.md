# Hi 👋🏾, I'm Andre Simamora

<p><img src="https://github-readme-stats.vercel.app/api?username=andriannus&show_icons=true&theme=dark&locale=en" alt="andriannus" /></p>

## About Me

```javascript
import { defineComponent, onMounted, reactive } from "vue";

export default defineComponent({
  name: "AboutMe",

  setup() {
    const state = reactive({
      currentWorkplace: {},
      dailyKnowledges: [],
      fullName: "",
    });

    onMounted(() => {
      setFullName();
      setDailyKnowledges();
      setCurrentWorkplace();
    });

    const setFullName = () => {
      state.fullName = "Andriannus Parasian";
    };

    const setCurrentWorkplace = () => {
      state.currentWorkplace = {
        company: "Tunaiku",
        position: "Front End Engineer",
      };
    };

    const setDailyKnowledges = () => {
      state.dailyKnowledges = [
        "TypeScript",
        "JavaScript",
        "Angular",
        "Vue",
        "AJAX",
        "CSS Preprocessor",
        "Jasmine",
        "Karma",
      ];
    };

    return { state };
  },
});
```

### Connect with me

<p align="left">
<a href="https://andriannus.id" target="blank"><img align="center" src="https://cdn.jsdelivr.net/npm/simple-icons@3.0.1/icons/googlechrome.svg" alt="andriannus" height="30" width="40" /></a>
<a href="https://linkedin.com/in/andriannus" target="blank"><img align="center" src="https://cdn.jsdelivr.net/npm/simple-icons@3.0.1/icons/linkedin.svg" alt="andriannus" height="30" width="40" /></a>
<a href="https://instagram.com/andriannus" target="blank"><img align="center" src="https://cdn.jsdelivr.net/npm/simple-icons@3.0.1/icons/instagram.svg" alt="andriannus" height="30" width="40" /></a>
<a href="https://twitter.com/andriannus" target="blank"><img align="center" src="https://cdn.jsdelivr.net/npm/simple-icons@3.0.1/icons/twitter.svg" alt="andriannus" height="30" width="40" /></a>
<a href="https://facebook.com/andriannus.p" target="blank"><img align="center" src="https://cdn.jsdelivr.net/npm/simple-icons@3.0.1/icons/facebook.svg" alt="andriannus.p" height="30" width="40" /></a>
</p>
