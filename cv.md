# rsschool-cv

## Selyakova Elizaveta

## Frontend Developer

## Contact information:

* **Phone:** +7 999 526 98 43
* **E-mail:** gasayliza@gamil.com
* **GitHub:** [Gasay-Liza](https://github.com/Gasay-Liza)
* **Telegram** [Selyakova Elizaveta](https://t.me/gasayliza)
* **Leetcode** [Gasay-Liza](https://leetcode.com/u/Gasay-Liza/)
* **Hexlet** [Selyakova Elizaveta](https://ru.hexlet.io/u/gasay-liza)

## About Me

I am 25 years old and began my career as a design engineer. In 2023, I completed web development courses and worked as a
front-end developer at the website and mobile application development studio 'Request Design'. Currently, I am
developing interfaces using React in Cherepovets at the company 'Northis'. I am continuously improving my skills by
solving algorithmic challenges on LeetCode and studying programming independently on Hexlet.

## Skills
* React, Redux Toolkit;
* JavaScript & TypeScript;
* Git, GitHub, GitLab;
* HTML5, CSS3;
* REST API, GraphQL;
* Material UI;
* Node.js, Express.js;
* Postman, MongoDB;
* Figma(for web development);

## Code example
*An example of my solution to an algorithmic problem on [Leetcode](https://leetcode.com/problems/balance-a-binary-search-tree/description/)*
```
function balanceBST(root: TreeNode | null): TreeNode | null {
    const nodeValues = [];
    function dfs(node: TreeNode | null) {
        if (!node) {
            return
        }
        dfs(node.left);
        nodeValues.push(node.val)
        dfs(node.right);
    }
    nodeValues.sort((a, b) => b - a);
    dfs(root);
    return createBalancedBst(nodeValues, 0, nodeValues.length - 1)


    function createBalancedBst(array: number[], start: number, end: number): TreeNode | null {
        if (start > end) {
            return null
        }
        const mid = start + Math.floor((end - start) / 2);
        const leftSubtree = createBalancedBst(array, start, mid - 1)
        const rightSubtree = createBalancedBst(array, mid + 1, end)

        const node = new TreeNode(array[mid], leftSubtree, rightSubtree);
        return node;
    }
};
```
# Experience

# Education
* **Bachelor, St. Petersburg Mining University**
* **Practicum Yandex** -  web developer courses
* **[Hexlet](https://ru.hexlet.io/u/gasay-liza)** 

# Languages

* **Russian** - native speaker.
* **English** - A2.