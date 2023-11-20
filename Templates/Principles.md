<%*
let rows = []
for (const [k, v] of Object.entries(tp.frontmatter.principles)) {
	rows.push([k, v])
}
rows.unshift(["Principle", "Summary"], [":--", ":--"])
rows = rows.map(x => (["", ...x, ""].join("|")))
tR += rows.join("\n") + "\n"
%>