<template>
  <QuestionCard :questionList="questionList"></QuestionCard>
</template>

<script>
import QuestionPage from './components/QuestionPage';
import QuestionList from './components/QuestionList';
import QuestionCard from './components/QuestionCard';

export default {
  name: 'App',
  components: {
    QuestionPage,
    QuestionList,
    QuestionCard
  },
  data: () => ({
    questionList: [
      {
        images: 'https://images-na.ssl-images-amazon.com/images/I/618v1Ud9ZeL._SX425_.jpg',
        choices: ["Heisenberg", "Michael Corleone", "Saul Goodman", "Gus Fring"],
        correctAnswer: "Heisenberg"
      },
      {
        images: 'https://vignette.wikia.nocookie.net/rickandmorty/images/a/a6/Rick_Sanchez.png/revision/latest?cb=20160923150728',
        choices: ["Beth Sanchez", "Fleep Floop", "Bird Person", "Rick Sanchez"],
        correctAnswer: "Rick Sanchez"
      },
      {
        images: 'https://res.cloudinary.com/wnotw/image/upload/c_limit,w_1536,q_auto:best,f_auto/v1512886004/ncqnyskqzivn4mbajufg',
        choices: ["Johnny Bravo", "Samurai Jack", "Scooby Doo", "Suzy"],
        correctAnswer: "Johnny Bravo"
      },
      {
        images: 'http://s3.amazonaws.com/assets.piedpiper.pro/app/uploads/2017/05/Richard-403-Blog.jpg',
        choices: ["Hitler", "Erlich Bachman", "Jian Yang", "Richard Hendricks"],
        correctAnswer: "Richard Hendricks"
      },
      {
        images: 'http://www.elcbrands.com/media/superman1.1.jpg',
        choices: ["Superman", "Thor", "Captain America", "Wonder Woman"],
        correctAnswer: "Superman"
      },
      {
        images: 'https://www.dccomics.com/sites/default/files/Char_GetToKnow_Batman80_5ca54cb83a27a6.53173051.png',
        choices: ["Ironman", "Batman", "Joker", "Lex Luthor"],
        correctAnswer: "Batman"
      },
      {
        images: 'https://vignette.wikia.nocookie.net/marveldatabase/images/9/92/Peter_Parker_%28Earth-30847%29_from_Marvel_vs._Capcom_Infinite_0001.png/revision/latest?cb=20170922195944',
        choices: ["Antman", "Night Monkey", "Spiderman", "Venom"],
        correctAnswer: "Spiderman"
      },
      {
        images: 'https://upload.wikimedia.org/wikipedia/en/thumb/d/d5/Aidan_Gillen_playing_Petyr_Baelish.jpg/220px-Aidan_Gillen_playing_Petyr_Baelish.jpg',
        choices: ["Jon Snow", "Petyr Baelish", "Tywin Lannister", "Tyrion Lannister"],
        correctAnswer: "Petyr Baelish"
      },
      {
        images: 'https://hips.hearstapps.com/digitalspyuk.cdnds.net/17/36/1504869306-bojack-horseman.jpg?crop=0.563xw:1.00xh;0.202xw,0&resize=480:*',
        choices: ["Princess Carolyn", "Todd Chavez", "BoJack Horseman", "Diane Nguyen"],
        correctAnswer: "Bojack Horseman"
      },
      {
        images: 'https://i.pinimg.com/originals/fd/ca/5a/fdca5a64c3046871c62be1b024e31651.png',
        choices: ["Zeus", "Barbie", "Hercules", "Pegasus"],
        correctAnswer: "Hercules"
      }
    ]
  })
};
</script>
