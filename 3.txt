// වචන ලැයිස්තුව (Data)
const slangData = {
    "ගොඩා": "වැඩියෙන් වැඩ කරන හෝ පාඩම් කරන පුද්ගලයා",
    "කුප්පිය": "කණ්ඩායමක් එකතු වී කරන කුඩා පාඩම් සාකච්ඡාව",
    "කැපීම": "දේශනයකට සහභාගී නොවී මඟ හැරීම",
    "බකට් එක": "විශ්වවිද්‍යාලයේදී ලැබෙන සාමූහික දඬුවම හෝ කරදරකාරී අවස්ථාව"
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