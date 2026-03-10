// වචන ලැයිස්තුව (Data)
const slangData = {
    "බාලගිරිය": "SCIENCE හී බෝජනාගාරය ",
    "කුප්පිය": "කණ්ඩායමක් එකතු වී කරන කුඩා පාඩම් සාකච්ඡාව",
    "බවන" : "UCSC හී බෝජනාගාරය "
};

function searchWord() {
    let input = document.getElementById("searchInput").value.trim();
    let resultArea = document.getElementById("resultArea");

    if (slangData[input]) {
        resultArea.innerHTML = `<h3>${input}</h3><p>${slangData[input]}</p>`;
    } else {
        resultArea.innerHTML = `<p style="color:red;">සමාවන්න, එම වචනය අපේ ශබ්දකෝෂයේ නැත.</p>`;
    }
}