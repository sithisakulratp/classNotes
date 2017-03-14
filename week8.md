# Week 8 (03.13.2017)
## Thyme Leaf
```markdown
@Controller
public class GreetingController {
@RequestMapping("/greeting")
public String greeting(@RequestParam(value="name", required=false, defaultValue="World")
    String name,
    @PathVariable(value = " city", required = false) String x, Model model) {
    model.addAttribute("name", name);
    model.addAttribute("city", x);
    return "greeting"; //the string name of the template (under 'templates' folder, which is under resources)
}

Request vs. path variables
 - the path variable - HTTP://LocalHost/greeting/dan/1/5/
 - request variable - /greeting?name=dan&bar=1
    - this is asking for the requestParam
 **Path parameter has to be before the request param**
 
- Ctrl + C = terminate the bootrun
```
