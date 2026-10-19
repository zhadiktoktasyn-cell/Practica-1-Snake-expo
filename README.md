import {
  View,
  Text,
  Image,
  StyleSheet,
  SafeAreaView,
  StatusBar,
} from 'react-native';

export default function App() {
  return (
    <SafeAreaView style={styles.container}>
      <StatusBar barStyle="light-content" />

      <View style={styles.card}>
  <Image
    source={require('./assets/GG.png')}
    style={styles.avatar}
  />

        <Text style={styles.name}>Токтасын Жадыгер</Text>

        <Text style={styles.group}>Группа: АЖ-401</Text>

        <View style={styles.divider} />

        <Text style={styles.label}>Электронная почта</Text>
        <Text style={styles.info}>zadik.toktasyn@gmail.com</Text>

        <Text style={styles.label}>О себе</Text>
        <Text style={styles.info}>
          Студент направления «Информационные системы».
          {'\n'}Интересуюсь мобильной разработкой и современными технологиями.
        </Text>

        <Text style={styles.label}>Хобби</Text>
        <Text style={styles.info}>
          💻 Программирование  🎮 Игры  🎵 Музыка
        </Text>

        <View style={styles.quote}>
          <Text style={styles.quoteText}>
            «Учись сегодня — создавай завтра.»
          </Text>
        </View>
      </View>
    </SafeAreaView>
  );
}

const styles = StyleSheet.create({
  container: {
    flex: 1,
    backgroundColor: '#1E293B',
  },

  card: {
    flex: 1,
    alignItems: 'center',
    justifyContent: 'center',
    paddingHorizontal: 25,
  },

  avatar: {
    width: 140,
    height: 140,
    borderRadius: 70,
    marginBottom: 20,
    borderWidth: 4,
    borderColor: '#FFFFFF',
  },

  name: {
    fontSize: 28,
    fontWeight: 'bold',
    color: '#FFFFFF',
    marginBottom: 8,
  },

  group: {
    fontSize: 18,
    color: '#CBD5E1',
  },

  divider: {
    width: '80%',
    height: 1,
    backgroundColor: '#64748B',
    marginVertical: 25,
  },

  label: {
    fontSize: 14,
    color: '#94A3B8',
    marginTop: 12,
    marginBottom: 4,
  },

  info: {
    fontSize: 16,
    color: '#F8FAFC',
    textAlign: 'center',
    lineHeight: 24,
  },

  quote: {
    marginTop: 25,
    padding: 15,
    borderRadius: 12,
    backgroundColor: '#334155',
  },

  quoteText: {
    color: '#E2E8F0',
    fontSize: 15,
    fontStyle: 'italic',
    textAlign: 'center',
  },
});
