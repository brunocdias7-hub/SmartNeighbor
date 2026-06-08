import { StatusBar } from 'expo-status-bar';
import { StyleSheet, Text, View, ScrollView, SafeAreaView } from
'react-native';
export default function App() {
return (
<SafeAreaView style={styles.safeContainer}>
<ScrollView contentContainerStyle={styles.container}>
<Text style={styles.headerTitle}>SmartNeighbor</Text>
<Text style={styles.subtitle}>Painel de Ajuda Comunitária de
Carapicuíba</Text>
<View style={styles.card}>
<Text style={styles.cardTitle}>Pedido #041 - Compra de
Medicamentos</Text>
<Text style={styles.cardDesc}>Solicitante: Sra. Maria (82
anos). Necessita buscar receita médica na Farmácia Popular do centro.</
Text>
<Text style={styles.tagUrgent}>URGENTE</Text>
</View>
<View style={styles.card}>
<Text style={styles.cardTitle}>Pedido #042 - Auxílio
Computacional</Text>
<Text style={styles.cardDesc}>Solicitante: Seu Jorge.
Necessita de auxílio para emitir a segunda via de boleto de energia.</
Text>
<Text style={styles.tagNormal}>ROTINA</Text>
</View>
<StatusBar style="auto" />
</ScrollView>
</SafeAreaView>
);
}
const styles = StyleSheet.create({
safeContainer: {
flex: 1,
backgroundColor: '#f4f6f9',
},
container: {
padding: 20,
alignItems: 'stretch',
},
headerTitle: {
fontSize: 26,
fontWeight: 'bold',
color: '#1a1a1a',
textAlign: 'center',
marginTop: 10,
},
subtitle: {
fontSize: 14,
color: '#666666',
textAlign: 'center',
marginBottom: 25,
},
card: {
backgroundColor: '#ffffff',
borderRadius: 8,
padding: 15,
marginBottom: 15,
borderWidth: 1,
borderColor: '#e0e0e0',
},
cardTitle: {
fontSize: 16,
fontWeight: 'bold',
color: '#333333',
marginBottom: 5,
},
cardDesc: {
fontSize: 13,
color: '#555555',
lineHeight: 18,
marginBottom: 10,
},
tagUrgent: {
alignSelf: 'flex-start',
backgroundColor: '#ffdddd',
color: '#cc0000',
fontSize: 11,
fontWeight: 'bold',
paddingVertical: 4,
paddingHorizontal: 8,
borderRadius: 4,
},
tagNormal: {
alignSelf: 'flex-start',
backgroundColor: '#e2f0d9',
color: '#385723',
fontSize: 11,
fontWeight: 'bold',
paddingVertical: 4,
paddingHorizontal: 8,